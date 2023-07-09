# Comparing `tmp/AshCrypt-1.3.4.tar.gz` & `tmp/AshCrypt-1.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AshCrypt-1.3.4.tar", last modified: Sun Jul  9 12:40:53 2023, max compression
+gzip compressed data, was "AshCrypt-1.3.5.tar", last modified: Sun Jul  9 22:31:08 2023, max compression
```

## Comparing `AshCrypt-1.3.4.tar` & `AshCrypt-1.3.5.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxrwx   0        0        0        0 2023-07-09 12:40:53.070354 AshCrypt-1.3.4/
-drwxrwxrwx   0        0        0        0 2023-07-09 12:40:53.015336 AshCrypt-1.3.4/AshCrypt/
--rw-rw-rw-   0        0        0     4985 2023-07-07 17:08:02.000000 AshCrypt-1.3.4/AshCrypt/Ash.py
--rw-rw-rw-   0        0        0    37332 2023-07-07 18:14:16.000000 AshCrypt-1.3.4/AshCrypt/AshCryptGUI.py
--rw-rw-rw-   0        0        0     6654 2023-07-01 17:13:11.000000 AshCrypt-1.3.4/AshCrypt/CliCrypt.py
--rw-rw-rw-   0        0        0     8450 2023-07-03 21:05:38.000000 AshCrypt-1.3.4/AshCrypt/Database.py
--rw-rw-rw-   0        0        0     3849 2023-07-01 02:35:10.000000 AshCrypt-1.3.4/AshCrypt/FileCrypt.py
--rw-rw-rw-   0        0        0    18439 2023-07-02 19:28:42.000000 AshCrypt-1.3.4/AshCrypt/README.md
--rw-rw-rw-   0        0        0     1852 2023-07-01 02:35:10.000000 AshCrypt-1.3.4/AshCrypt/TextCrypt.py
--rw-rw-rw-   0        0        0       88 2023-07-03 12:24:38.000000 AshCrypt-1.3.4/AshCrypt/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-09 12:40:53.053665 AshCrypt-1.3.4/AshCrypt/__pycache__/
--rw-rw-rw-   0        0        0     6336 2023-07-03 12:24:42.000000 AshCrypt-1.3.4/AshCrypt/__pycache__/Ash.cpython-39.pyc
--rw-rw-rw-   0        0        0    19834 2023-07-03 21:09:38.000000 AshCrypt-1.3.4/AshCrypt/__pycache__/AshCryptGUI.cpython-39.pyc
--rw-rw-rw-   0        0        0     7285 2023-07-03 21:09:38.000000 AshCrypt-1.3.4/AshCrypt/__pycache__/Database.cpython-39.pyc
--rw-rw-rw-   0        0        0     3236 2023-07-01 17:13:25.000000 AshCrypt-1.3.4/AshCrypt/__pycache__/FileCrypt.cpython-39.pyc
--rw-rw-rw-   0        0        0     2409 2023-07-01 17:13:25.000000 AshCrypt-1.3.4/AshCrypt/__pycache__/TextCrypt.cpython-39.pyc
--rw-rw-rw-   0        0        0      218 2023-07-03 12:24:42.000000 AshCrypt-1.3.4/AshCrypt/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0      779 2023-07-07 12:45:40.000000 AshCrypt-1.3.4/AshCrypt/__pycache__/qr.cpython-39.pyc
--rw-rw-rw-   0        0        0      536 2023-07-07 12:45:35.000000 AshCrypt-1.3.4/AshCrypt/qr.py
-drwxrwxrwx   0        0        0        0 2023-07-09 12:40:53.059756 AshCrypt-1.3.4/AshCrypt/unittests/
--rw-rw-rw-   0        0        0       25 2023-06-30 15:01:03.000000 AshCrypt-1.3.4/AshCrypt/unittests/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-09 12:40:53.066348 AshCrypt-1.3.4/AshCrypt/unittests/__pycache__/
--rw-rw-rw-   0        0        0      173 2023-07-02 16:55:47.000000 AshCrypt-1.3.4/AshCrypt/unittests/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0     5782 2023-07-03 12:24:42.000000 AshCrypt-1.3.4/AshCrypt/unittests/__pycache__/unittestAsh.cpython-39.pyc
--rw-rw-rw-   0        0        0     3395 2023-07-03 12:52:55.000000 AshCrypt-1.3.4/AshCrypt/unittests/unittestAsh.py
-drwxrwxrwx   0        0        0        0 2023-07-09 12:40:53.031857 AshCrypt-1.3.4/AshCrypt.egg-info/
--rw-rw-rw-   0        0        0    19466 2023-07-09 12:40:52.000000 AshCrypt-1.3.4/AshCrypt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      853 2023-07-09 12:40:52.000000 AshCrypt-1.3.4/AshCrypt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-09 12:40:52.000000 AshCrypt-1.3.4/AshCrypt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       70 2023-07-09 12:40:52.000000 AshCrypt-1.3.4/AshCrypt.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-09 12:40:52.000000 AshCrypt-1.3.4/AshCrypt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1091 2023-06-30 15:01:03.000000 AshCrypt-1.3.4/LICENSE
--rw-rw-rw-   0        0        0    19466 2023-07-09 12:40:53.069349 AshCrypt-1.3.4/PKG-INFO
--rw-rw-rw-   0        0        0    21819 2023-07-07 14:29:17.000000 AshCrypt-1.3.4/README.md
--rw-rw-rw-   0        0        0       42 2023-07-09 12:40:53.070354 AshCrypt-1.3.4/setup.cfg
--rw-rw-rw-   0        0        0     1660 2023-07-07 14:06:29.000000 AshCrypt-1.3.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-09 22:31:08.122261 AshCrypt-1.3.5/
+drwxrwxrwx   0        0        0        0 2023-07-09 22:31:08.086271 AshCrypt-1.3.5/AshCrypt/
+-rw-rw-rw-   0        0        0     5209 2023-07-09 22:22:00.000000 AshCrypt-1.3.5/AshCrypt/Ash.py
+-rw-rw-rw-   0        0        0    39532 2023-07-09 22:23:47.000000 AshCrypt-1.3.5/AshCrypt/AshCryptGUI.py
+-rw-rw-rw-   0        0        0     6704 2023-07-09 22:26:42.000000 AshCrypt-1.3.5/AshCrypt/CliCrypt.py
+-rw-rw-rw-   0        0        0     8993 2023-07-09 22:27:03.000000 AshCrypt-1.3.5/AshCrypt/Database.py
+-rw-rw-rw-   0        0        0     4019 2023-07-09 22:27:54.000000 AshCrypt-1.3.5/AshCrypt/FileCrypt.py
+-rw-rw-rw-   0        0        0    18439 2023-07-02 19:28:42.000000 AshCrypt-1.3.5/AshCrypt/README.md
+-rw-rw-rw-   0        0        0     1801 2023-07-09 22:29:17.000000 AshCrypt-1.3.5/AshCrypt/TextCrypt.py
+-rw-rw-rw-   0        0        0       88 2023-07-03 12:24:38.000000 AshCrypt-1.3.5/AshCrypt/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-09 22:31:08.110628 AshCrypt-1.3.5/AshCrypt/__pycache__/
+-rw-rw-rw-   0        0        0     6384 2023-07-09 22:24:31.000000 AshCrypt-1.3.5/AshCrypt/__pycache__/Ash.cpython-39.pyc
+-rw-rw-rw-   0        0        0    19834 2023-07-03 21:09:38.000000 AshCrypt-1.3.5/AshCrypt/__pycache__/AshCryptGUI.cpython-39.pyc
+-rw-rw-rw-   0        0        0     7285 2023-07-03 21:09:38.000000 AshCrypt-1.3.5/AshCrypt/__pycache__/Database.cpython-39.pyc
+-rw-rw-rw-   0        0        0     3236 2023-07-01 17:13:25.000000 AshCrypt-1.3.5/AshCrypt/__pycache__/FileCrypt.cpython-39.pyc
+-rw-rw-rw-   0        0        0     2409 2023-07-01 17:13:25.000000 AshCrypt-1.3.5/AshCrypt/__pycache__/TextCrypt.cpython-39.pyc
+-rw-rw-rw-   0        0        0      218 2023-07-03 12:24:42.000000 AshCrypt-1.3.5/AshCrypt/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0      779 2023-07-07 12:45:40.000000 AshCrypt-1.3.5/AshCrypt/__pycache__/qr.cpython-39.pyc
+-rw-rw-rw-   0        0        0      536 2023-07-09 22:29:03.000000 AshCrypt-1.3.5/AshCrypt/qr.py
+drwxrwxrwx   0        0        0        0 2023-07-09 22:31:08.114964 AshCrypt-1.3.5/AshCrypt/unittests/
+-rw-rw-rw-   0        0        0       25 2023-06-30 15:01:03.000000 AshCrypt-1.3.5/AshCrypt/unittests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-09 22:31:08.119046 AshCrypt-1.3.5/AshCrypt/unittests/__pycache__/
+-rw-rw-rw-   0        0        0      173 2023-07-02 16:55:47.000000 AshCrypt-1.3.5/AshCrypt/unittests/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0     5782 2023-07-03 12:24:42.000000 AshCrypt-1.3.5/AshCrypt/unittests/__pycache__/unittestAsh.cpython-39.pyc
+-rw-rw-rw-   0        0        0     3395 2023-07-03 12:52:55.000000 AshCrypt-1.3.5/AshCrypt/unittests/unittestAsh.py
+drwxrwxrwx   0        0        0        0 2023-07-09 22:31:08.095877 AshCrypt-1.3.5/AshCrypt.egg-info/
+-rw-rw-rw-   0        0        0    19466 2023-07-09 22:31:07.000000 AshCrypt-1.3.5/AshCrypt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      853 2023-07-09 22:31:07.000000 AshCrypt-1.3.5/AshCrypt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-09 22:31:07.000000 AshCrypt-1.3.5/AshCrypt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       70 2023-07-09 22:31:07.000000 AshCrypt-1.3.5/AshCrypt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-09 22:31:07.000000 AshCrypt-1.3.5/AshCrypt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1091 2023-06-30 15:01:03.000000 AshCrypt-1.3.5/LICENSE
+-rw-rw-rw-   0        0        0    19466 2023-07-09 22:31:08.122261 AshCrypt-1.3.5/PKG-INFO
+-rw-rw-rw-   0        0        0    21825 2023-07-09 20:32:48.000000 AshCrypt-1.3.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-09 22:31:08.123261 AshCrypt-1.3.5/setup.cfg
+-rw-rw-rw-   0        0        0     1660 2023-07-09 20:20:19.000000 AshCrypt-1.3.5/setup.py
```

### Comparing `AshCrypt-1.3.4/AshCrypt/Ash.py` & `AshCrypt-1.3.5/AshCrypt/Ash.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,19 +5,21 @@
 from typing import Union
 import hmac as hmc
 import bcrypt
 import base64
 import struct
 import os
 
+
 class IterationsOutofaRangeError(Exception):
-    def __init__(self,num : any)->None:
+    def __init__(self, num: any) -> None:
         self.display = f'Iterations must be between 50 and 100000. RECEIVED : {num} '
         super().__init__(self.display)
 
+
 class Enc:
     def __init__(self, message: Union[str, bytes], mainkey: str) -> None:
         if isinstance(message, str):
             self.message = message.encode()
         elif isinstance(message, bytes):
             self.message = message
 
@@ -30,63 +32,70 @@
             raise IterationsOutofaRangeError(self.iterations)
         self.encKey = self.derkey(self.mainkey, self.salt, self.iterations)
         self.hmac_key = self.derkey(self.mainkey, self.pepper, self.iterations)
 
     @staticmethod
     def derkey(mainkey: str, salt_pepper: bytes, iterations: int) -> bytes:
         return bcrypt.kdf(
-            password = mainkey.encode('UTF-8'),
-            salt = salt_pepper,
-            desired_key_bytes = 32,
-            rounds = iterations)
+            password=mainkey.encode('UTF-8'),
+            salt=salt_pepper,
+            desired_key_bytes=32,
+            rounds=iterations)
 
     @staticmethod
-    def genMainkey()->str:
+    def genMainkey() -> str:
         return os.urandom(64).hex()
 
     def mode(self):
         return modes.CBC(self.iv)
 
     def cipher(self):
-     return Cipher(algorithms.AES(key=self.encKey), mode=self.mode(), backend=default_backend())
+        return Cipher(
+            algorithms.AES(
+                key=self.encKey),
+            mode=self.mode(),
+            backend=default_backend())
 
     def cipher_encryptor(self):
         return self.cipher().encryptor()
 
     def padded_message(self) -> bytes:
         padder = padding.PKCS7(128).padder()
         return padder.update(self.message) + padder.finalize()
 
     def ciphertext(self) -> bytes:
-        return self.cipher_encryptor().update(self.padded_message()) + self.cipher_encryptor().finalize()
+        return self.cipher_encryptor().update(self.padded_message()) + \
+            self.cipher_encryptor().finalize()
 
-    def HMAC(self) ->bytes:
+    def HMAC(self) -> bytes:
         h = self.hmac_key
         h = hmac.HMAC(h, hashes.SHA512())
         h.update(self.ciphertext())
         return h.finalize()
 
-    def setupIterations(self)->bytes:
-        iters_bytes = struct.pack('!I',self.iterations)
+    def setupIterations(self) -> bytes:
+        iters_bytes = struct.pack('!I', self.iterations)
         return iters_bytes
 
     def encToBytes(self) -> bytes:
-        return self.HMAC() + self.iv + self.salt + self.pepper + self.setupIterations() + self.ciphertext()
+        return self.HMAC() + self.iv + self.salt + self.pepper + \
+            self.setupIterations() + self.ciphertext()
 
     def encToStr(self) -> str:
         return base64.urlsafe_b64encode(self.encToBytes()).decode('UTF-8')
 
 
 class MessageTamperingError(Exception):
-    def __init__(self)->None:
+    def __init__(self) -> None:
         self.display = 'HMAC mismatch ! Message has been TAMPERED with ,\n or Possible key difference'
         super().__init__(self.display)
 
+
 class Dec:
-    def __init__(self,message: Union[str, bytes], mainkey: str)->None:
+    def __init__(self, message: Union[str, bytes], mainkey: str) -> None:
         if isinstance(message, str):
             m = message.encode('UTF-8')
             self.message = base64.urlsafe_b64decode(m)
         elif isinstance(message, bytes):
             self.message = message
         self.key = mainkey
         self.rec_hmac = self.message[:64]
@@ -94,40 +103,49 @@
         self.rec_salt = self.message[80:96]
         self.rec_pepper = self.message[96:112]
         self.rec_iterations = struct.unpack('!I', self.message[112:116])[0]
         if self.rec_iterations < 50 or self.rec_iterations > 100000:
             raise IterationsOutofaRangeError(self.rec_iterations)
         self.rec_ciphertext = self.message[116:]
         self.decKey = Enc.derkey(self.key, self.rec_salt, self.rec_iterations)
-        self.hmac_k = Enc.derkey(self.key, self.rec_pepper, self.rec_iterations)
-        if self.verifyHMAC() is False :
+        self.hmac_k = Enc.derkey(
+            self.key,
+            self.rec_pepper,
+            self.rec_iterations)
+        if self.verifyHMAC() is False:
             raise MessageTamperingError()
-    def actualHMAC(self)->bytes:
+
+    def actualHMAC(self) -> bytes:
         h = self.hmac_k
         h = hmac.HMAC(h, hashes.SHA512())
         h.update(self.rec_ciphertext)
         return h.finalize()
 
-    def verifyHMAC(self)->bool:
+    def verifyHMAC(self) -> bool:
         return hmc.compare_digest(self.actualHMAC(), self.rec_hmac)
 
     def mode(self):
         return modes.CBC(self.rec_iv)
 
     def cipher(self):
-        return Cipher(algorithms.AES(key=self.decKey), mode=self.mode(), backend=default_backend())
+        return Cipher(
+            algorithms.AES(
+                key=self.decKey),
+            mode=self.mode(),
+            backend=default_backend())
 
     def cipher_decryptor(self):
         return self.cipher().decryptor()
 
     def pre_unpadding_dec(self) -> bytes:
-        return self.cipher_decryptor().update(self.rec_ciphertext) + self.cipher_decryptor().finalize()
+        return self.cipher_decryptor().update(self.rec_ciphertext) + \
+            self.cipher_decryptor().finalize()
 
-    def unpadded_m(self)->bytes:
+    def unpadded_m(self) -> bytes:
         unpadder = padding.PKCS7(128).unpadder()
         return unpadder.update(self.pre_unpadding_dec()) + unpadder.finalize()
 
-    def decToBytes(self)->bytes:
+    def decToBytes(self) -> bytes:
         return self.unpadded_m()
 
     def decToStr(self) -> str:
         return (self.unpadded_m().decode('UTF-8'))
```

### Comparing `AshCrypt-1.3.4/AshCrypt/AshCryptGUI.py` & `AshCrypt-1.3.5/AshCrypt/AshCryptGUI.py`

 * *Files 17% similar despite different names*

```diff
@@ -11,310 +11,368 @@
 import json
 import re
 
 
 '''--------------------------------------FRAMING STARTED-------------------------------------------------------------'''
 
 object = tk.Window(themename='vapor')
-object.resizable(False ,False)
+object.resizable(False, False)
 object.title('AshCrypt')
 object.geometry('1500x800')
 
 
-databaseFrame = tk.Frame(master=object , width=500 , height=800)
-databaseFrame.place(x=0 , y=0)
+databaseFrame = tk.Frame(master=object, width=500, height=800)
+databaseFrame.place(x=0, y=0)
 
-frameFile1 = tk.Frame(master=object , width=500 , height=250)
-frameFile1.place(x=500 , y=0)
+frameFile1 = tk.Frame(master=object, width=500, height=250)
+frameFile1.place(x=500, y=0)
 
-frameFile2 = tk.Frame(master=object , width=500 , height=250)
-frameFile2.place(x=500 , y=250)
+frameFile2 = tk.Frame(master=object, width=500, height=250)
+frameFile2.place(x=500, y=250)
 
-textFrame1 = tk.Frame(master=object , width=500 , height=250)
-textFrame1.place(x=1000 , y=0)
+textFrame1 = tk.Frame(master=object, width=500, height=250)
+textFrame1.place(x=1000, y=0)
 
-textFrame2 = tk.Frame(master=object , width=500 , height=250)
-textFrame2.place(x=1000 , y=250)
+textFrame2 = tk.Frame(master=object, width=500, height=250)
+textFrame2.place(x=1000, y=250)
 
-lowerFrame = tk.Frame(master=object, width=1000 ,height=260)
-lowerFrame.place(x=500,y=540)
+lowerFrame = tk.Frame(master=object, width=1000, height=260)
+lowerFrame.place(x=500, y=540)
 
 '''--------------------------------------DATABASE FRAME STARTED------------------------------------------------'''
 
 
-databaseFrame = tk.Frame(master=object,height=800, width=500)
+databaseFrame = tk.Frame(master=object, height=800, width=500)
 databaseFrame.place(rely=0, relx=0)
 
-console_label = tk.Label(master=databaseFrame, text='DATABASE OUTPUT CONSOLE', font='Calibre 15 bold')
-console_label.place( relx=0.09,rely=0.04)
+console_label = tk.Label(
+    master=databaseFrame,
+    text='DATABASE OUTPUT CONSOLE',
+    font='Calibre 15 bold')
+console_label.place(relx=0.09, rely=0.04)
 
-import platform
 if platform.system() == 'Windows':
-    db_display_text = tk.Text(width=38 , height=18, font='Calibre 13 bold',wrap='word')
-    db_display_text.place(relx=0.015 ,rely=0.105)
-    db_display_text.insert(tk.END,'Waiting to fetch..')
+    db_display_text = tk.Text(
+        width=38,
+        height=18,
+        font='Calibre 13 bold',
+        wrap='word')
+    db_display_text.place(relx=0.015, rely=0.105)
+    db_display_text.insert(tk.END, 'Waiting to fetch..')
 else:
-    db_display_text = tk.Text(width=38, height=22, font='Calibre 13 bold', wrap='word')
+    db_display_text = tk.Text(
+        width=38,
+        height=22,
+        font='Calibre 13 bold',
+        wrap='word')
     db_display_text.place(relx=0.015, rely=0.105)
     db_display_text.insert(tk.END, 'Waiting to fetch..')
 
 
 def show_all_content():
-    global db_enable_blocker, main_db_name_var, usable_real_path, main_db_conn,db_display_text,keys_db_conn
+    global db_enable_blocker, main_db_name_var, usable_real_path, main_db_conn, db_display_text, keys_db_conn
     if db_enable_blocker != 0:
         db_display_text.delete('1.0', tk.END)
-        db_display_text.insert(tk.END, f"Check 'output.json' in the chosen path : {usable_real_path}\n")
+        db_display_text.insert(
+            tk.END, f"Check 'output.json' in the chosen path : {usable_real_path}\n")
         json_path = os.path.join(usable_real_path, 'output.json')
         if swich_db_var.get() == 1:
             conn = keys_db_conn
         else:
             conn = main_db_conn
         try:
             with open(json_path, 'w') as f:
                 eBuffer = {}
                 for e in conn.content():
-                    eBuffer['ID ' + e[0].__str__()] = [{'Filename': e[1]}, {'Content': e[2].__str__()}, {'KeyRef': e[3]}]
+                    eBuffer['ID ' + e[0].__str__()] = [{'Filename': e[1]}, {
+                        'Content': e[2].__str__()}, {'KeyRef': e[3]}]
                 eJSON = json.dumps(eBuffer, indent=2)
                 f.write(eJSON)
-                db_display_text.insert(tk.END,f"\nSuccessfully written all table content in output.json\n"
-                                              f"\nNote that this file will be deleted when the app is closed")
-        except:
-            db_display_text.insert(tk.END, f"Failed to write all table content in output.json\n")
-
+                db_display_text.insert(
+                    tk.END, f"\nSuccessfully written all table content in output.json\n"
+                    f"\nNote that this file will be deleted when the app is closed")
+        except BaseException:
+            db_display_text.insert(
+                tk.END, f"Failed to write all table content in output.json\n")
 
 
 def show_content_by_id():
-    global db_enable_blocker, main_db_conn,keys_db_conn, content_id_entry_var, usable_real_path
+    global db_enable_blocker, main_db_conn, keys_db_conn, content_id_entry_var, usable_real_path
     idd = content_id_entry_var.get().strip()
     last_id = checkid()
     if db_enable_blocker != 0:
         if swich_db_var.get() == 1:
             conn = keys_db_conn
         else:
             conn = main_db_conn
         try:
             if int(idd) > 0:
                 if last_id == -1:
                     db_display_text.delete('1.0', tk.END)
-                    db_display_text.insert(tk.END, 'The table does not have any content to show')
+                    db_display_text.insert(
+                        tk.END, 'The table does not have any content to show')
                 elif last_id != -1:
 
                     if int(idd) in range(1, last_id):
                         db_display_text.delete('1.0', tk.END)
-                        to_json_path = os.path.join(usable_real_path, 'output.json')
+                        to_json_path = os.path.join(
+                            usable_real_path, 'output.json')
                         with open(to_json_path, 'w') as f:
                             eBuffer = {}
                             for e in conn.content_by_id(int(idd)):
-                                eBuffer['ID_' + e[0].__str__()] = [{'Filename': e[1]}, {'Content': e[2].__str__()},
-                                                                   {'KeyRef': e[3]}]
+                                eBuffer['ID_' + e[0].__str__()] = [{'Filename': e[1]}, {
+                                    'Content': e[2].__str__()}, {'KeyRef': e[3]}]
                             eJSON = json.dumps(eBuffer, indent=2)
                             f.write(eJSON)
-                        db_display_text.insert(tk.END, f"Successful fetch !\n\nCheck the 'output.json' file in the"
-                                                       f" chosen path :\n\n'{usable_real_path}'")
+                        db_display_text.insert(
+                            tk.END, f"Successful fetch !\n\nCheck the 'output.json' file in the"
+                            f" chosen path :\n\n'{usable_real_path}'")
                     if int(idd) == last_id:
                         db_display_text.delete('1.0', tk.END)
                         db_display_text.insert(tk.END, 'Chosen last ID\n\n')
-                        to_json_path = os.path.join(usable_real_path,'output.json')
+                        to_json_path = os.path.join(
+                            usable_real_path, 'output.json')
                         try:
                             with open(to_json_path, 'w') as f:
                                 eBuffer = {}
                                 for e in conn.content_by_id(int(idd)):
-                                    eBuffer['ID_' + e[0].__str__()] = [{'Filename': e[1]}, {'Content': e[2].__str__()},
-                                                                       {'KeyRef': e[3]}]
+                                    eBuffer['ID_' + e[0].__str__()] = [{'Filename': e[1]}, {
+                                        'Content': e[2].__str__()}, {'KeyRef': e[3]}]
                                 eJSON = json.dumps(eBuffer, indent=2)
                                 f.write(eJSON)
-                            db_display_text.insert(tk.END, f"Successful fetch !\n\nCheck the 'output.json' file in the"
-                                                           f" the chosen path :\n\n'{usable_real_path}'")
-                        except:
+                            db_display_text.insert(
+                                tk.END, f"Successful fetch !\n\nCheck the 'output.json' file in the"
+                                f" the chosen path :\n\n'{usable_real_path}'")
+                        except BaseException:
                             db_display_text.delete('1.0', tk.END)
-                            db_display_text.insert(tk.END,"ERROR \n\nCheck the validity of 'output.json' file"
-                                                          "\n\nCheck if the database is faulty\n")
+                            db_display_text.insert(
+                                tk.END, "ERROR \n\nCheck the validity of 'output.json' file"
+                                "\n\nCheck if the database is faulty\n")
                     elif int(idd) > last_id:
                         db_display_text.delete('1.0', tk.END)
-                        db_display_text.insert(tk.END, 'Given ID is greater than the highest available ID')
+                        db_display_text.insert(
+                            tk.END, 'Given ID is greater than the highest available ID')
             else:
                 db_display_text.delete('1.0', tk.END)
-                db_display_text.insert(tk.END, 'ID must be strictly greater than 0')
-        except:
+                db_display_text.insert(
+                    tk.END, 'ID must be strictly greater than 0')
+        except BaseException:
             db_display_text.delete('1.0', tk.END)
             db_display_text.insert(tk.END, 'ID value must be a valid integer')
 
 
 def drop_content_by_id():
-    global db_enable_blocker,main_db_conn,keys_db_conn,content_id_entry_var
+    global db_enable_blocker, main_db_conn, keys_db_conn, content_id_entry_var
     idd = content_id_entry_var.get().strip()
     last_id = checkid()
     if db_enable_blocker != 0:
         if swich_db_var.get() == 1:
             conn = keys_db_conn
         else:
             conn = main_db_conn
         try:
             if int(idd) > 0:
                 if last_id == -1:
                     db_display_text.delete('1.0', tk.END)
-                    db_display_text.insert(tk.END,'The table does not have any content to drop')
-                elif last_id != -1 :
+                    db_display_text.insert(
+                        tk.END, 'The table does not have any content to drop')
+                elif last_id != -1:
 
-                    if int(idd) in range(1,last_id):
+                    if int(idd) in range(1, last_id):
                         db_display_text.delete('1.0', tk.END)
-                        db_display_text.insert(tk.END,'Valid ID')
+                        db_display_text.insert(tk.END, 'Valid ID')
                         conn.drop_content(idd)
-                        db_display_text.insert(tk.END, f'\nDropping by ID {idd} Went successful')
+                        db_display_text.insert(
+                            tk.END, f'\nDropping by ID {idd} Went successful')
 
                     if int(idd) == last_id:
                         db_display_text.delete('1.0', tk.END)
                         db_display_text.insert(tk.END, 'Chosen last ID')
                         conn.drop_content(idd)
-                        db_display_text.insert(tk.END, f'\nDropping by ID {idd} Went successful')
+                        db_display_text.insert(
+                            tk.END, f'\nDropping by ID {idd} Went successful')
 
                     elif int(idd) > last_id:
                         db_display_text.delete('1.0', tk.END)
-                        db_display_text.insert(tk.END, 'Given ID is greater than the highest available ID')
+                        db_display_text.insert(
+                            tk.END, 'Given ID is greater than the highest available ID')
             else:
                 db_display_text.delete('1.0', tk.END)
-                db_display_text.insert(tk.END, 'ID must be strictly greater than 0')
-        except:
+                db_display_text.insert(
+                    tk.END, 'ID must be strictly greater than 0')
+        except BaseException:
             db_display_text.delete('1.0', tk.END)
             db_display_text.insert(tk.END, 'ID value must be a valid integer')
 
 
+show_all_content_button = tk.Button(
+    master=databaseFrame,
+    text='SHOW ALL TABLE CONTENT',
+    command=show_all_content,
+    bootstyle='warning outline')
+show_all_content_button.place(relx=0.287, rely=0.87)
 
 
+query_clicks = 1
 
 
-show_all_content_button = tk.Button(master=databaseFrame,text='SHOW ALL TABLE CONTENT',command=show_all_content,bootstyle='warning outline')
-show_all_content_button.place(relx=0.287,rely=0.87)
-
-
-query_clicks = 1
 def query():
-    global db_enable_blocker,main_db_conn,keys_db_conn ,usable_real_path,query_clicks
-    if db_enable_blocker !=0 :
+    global db_enable_blocker, main_db_conn, keys_db_conn, usable_real_path, query_clicks
+    if db_enable_blocker != 0:
         if swich_db_var.get() == 1:
             conn = keys_db_conn
         else:
             conn = main_db_conn
         query_var = query_entry_var.get().strip()
         if len(query_var) > 0:
             try:
                 db_display_text.delete('1.0', tk.END)
-                json_file = os.path.join(usable_real_path,'output.json')
+                json_file = os.path.join(usable_real_path, 'output.json')
                 with open(json_file, 'w') as f:
                     query_out = conn.query(query_var)
                     conn.addtable()
-                    eJSON = json.dumps({f'query {query_clicks}': query_out}, indent=2)
+                    eJSON = json.dumps(
+                        {f'query {query_clicks}': query_out}, indent=2)
                     query_clicks += 1
                     f.write(eJSON)
-                db_display_text.insert(tk.END, f"Ran query {query_clicks} !\n\n")
-                db_display_text.insert(tk.END, f"The result of the query is in 'output.json' file\n\n")
-            except:
+                db_display_text.insert(
+                    tk.END, f"Ran query {query_clicks} !\n\n")
+                db_display_text.insert(
+                    tk.END, f"The result of the query is in 'output.json' file\n\n")
+            except BaseException:
                 db_display_text.delete('1.0', tk.END)
-                db_display_text.insert(tk.END, f"Failed to finish the query!\n\n")
-                db_display_text.insert(tk.END,'Detected object that is not JSON serializable\n\n')
-                db_display_text.insert(tk.END,'Use buttons instead if possible')
+                db_display_text.insert(
+                    tk.END, f"Failed to finish the query!\n\n")
+                db_display_text.insert(
+                    tk.END, 'Detected object that is not JSON serializable\n\n')
+                db_display_text.insert(
+                    tk.END, 'Use buttons instead if possible')
         else:
             db_display_text.delete('1.0', tk.END)
             db_display_text.insert(tk.END, f"Can't query nothing\n\n")
 
 
-
-
-
-
 query_entry_var = tk.StringVar()
-query_entry = tk.Entry(master=databaseFrame ,
-                        width=38,
-                        font='Calibre 13 bold',
-                        textvariable=query_entry_var).place(relx=0.043, rely=0.742)
-
-query_button = tk.Button(master=databaseFrame,text='RUN QUERY',command=query,bootstyle='warning outline')
-query_button.place(relx=0.39,rely=0.81)
-
-
-
-drop_content_by_id_button = tk.Button(master=databaseFrame,text='DROP CONTENT BY ID',command=drop_content_by_id,bootstyle='warning outline')
-drop_content_by_id_button.place(relx=0.08,rely=0.93)
+query_entry = tk.Entry(
+    master=databaseFrame,
+    width=38,
+    font='Calibre 13 bold',
+    textvariable=query_entry_var).place(
+        relx=0.043,
+    rely=0.742)
+
+query_button = tk.Button(
+    master=databaseFrame,
+    text='RUN QUERY',
+    command=query,
+    bootstyle='warning outline')
+query_button.place(relx=0.39, rely=0.81)
+
+
+drop_content_by_id_button = tk.Button(
+    master=databaseFrame,
+    text='DROP CONTENT BY ID',
+    command=drop_content_by_id,
+    bootstyle='warning outline')
+drop_content_by_id_button.place(relx=0.08, rely=0.93)
 
 content_id_entry_var = tk.StringVar(value=' ID')
-content_id_entry = tk.Entry(master=databaseFrame,textvariable=content_id_entry_var,width=3,font='Calibre 11')
-content_id_entry.place(relx=0.45,rely=0.93)
-
-show_content_by_id_button = tk.Button(master=databaseFrame,text='SHOW CONTENT BY ID',command=show_content_by_id,bootstyle='warning outline')
-show_content_by_id_button.place(relx=0.562,rely=0.93)
+content_id_entry = tk.Entry(
+    master=databaseFrame,
+    textvariable=content_id_entry_var,
+    width=3,
+    font='Calibre 11')
+content_id_entry.place(relx=0.45, rely=0.93)
+
+show_content_by_id_button = tk.Button(
+    master=databaseFrame,
+    text='SHOW CONTENT BY ID',
+    command=show_content_by_id,
+    bootstyle='warning outline')
+show_content_by_id_button.place(relx=0.562, rely=0.93)
 
 
 '''----------------------------------------LOWER FRAME STARTED----------------------------------'''
 
 
-
-lowerFrame = tk.Frame(master=object, width=1000 ,height=260)
-lowerFrame.place(x=500,y=540)
+lowerFrame = tk.Frame(master=object, width=1000, height=260)
+lowerFrame.place(x=500, y=540)
 
 
 db_path_blocker = 0
 usable_real_path = ''
+
+
 def set_db_path():
-    global db_path_blocker,usable_real_path
+    global db_path_blocker, usable_real_path
     path = db_path_var.get().strip()
-    if os.path.isdir(path.strip()) :
+    if os.path.isdir(path.strip()):
         db_path_blocker = 1
         db_path_result_var.set('SET')
         usable_real_path = path
-    else :
+    else:
         db_path_blocker = 0
         db_path_result_var.set('NOT SET')
         usable_real_path = ''
 
 
-
 main_db_name_blocker = 0
 db_already_exists_blocker = 0
 maindbname = ''
+
+
 def main_db_name():
     global main_db_name_blocker,\
         db_already_exists_blocker,\
-        usable_real_path,db_path_blocker,\
+        usable_real_path, db_path_blocker,\
         success_maindb_connection_blocker,\
         main_db_conn,\
         maindbname
 
     dbname = main_db_name_var.get().strip()
     if re.match(r'((^[\w(-.)?]+\.db$)|(^[\w?(-.)]\.db$))', dbname):
         try:
             maindbname = dbname
             main_db_name_blocker = 1
             main_db_name_result_var.set('SET')
             if db_path_blocker == 1:
                 fullpath = usable_real_path
                 conn_path_db = os.path.join(usable_real_path, maindbname)
-                if os.path.isfile(fullpath + f'\\{maindbname}') or os.path.isfile(fullpath + f'/{maindbname}')  :
+                if os.path.isfile(
+                        fullpath +
+                        f'\\{maindbname}') or os.path.isfile(
+                        fullpath +
+                        f'/{maindbname}'):
                     db_already_exists_blocker = 1
                     main_db_conn = AD.Database(conn_path_db)
                     main_db_conn.addtable()
                     main_db_name_result_var.set('CONNECTED')
                     db_display_text.delete('1.0', tk.END)
-                    db_display_text.insert(tk.END, f'Connected to {maindbname}..\n\n')
+                    db_display_text.insert(
+                        tk.END, f'Connected to {maindbname}..\n\n')
                     success_maindb_connection_blocker = 1
                     encfiletoolbutt.state(['!disabled'])
                     decfiletoolbutt.state(['!disabled'])
                 else:
                     db_already_exists_blocker = 0
                     main_db_conn = AD.Database(conn_path_db)
                     main_db_conn.addtable()
                     db_display_text.delete('1.0', tk.END)
-                    db_display_text.insert(tk.END, f"Created and Connected to '{maindbname}'.. in the directory '{fullpath}'\n\n")
+                    db_display_text.insert(
+                        tk.END,
+                        f"Created and Connected to '{maindbname}'.. in the directory '{fullpath}'\n\n")
                     success_maindb_connection_blocker = 1
                     encfiletoolbutt.state(['!disabled'])
                     decfiletoolbutt.state(['!disabled'])
 
             else:
                 db_display_text.delete('1.0', tk.END)
-                db_display_text.insert(tk.END, f"PATH : '{db_path_var.get().strip()}' is not a valid path\n\n")
-        except:
+                db_display_text.insert(
+                    tk.END, f"PATH : '{db_path_var.get().strip()}' is not a valid path\n\n")
+        except BaseException:
             db_display_text.delete('1.0', tk.END)
             db_display_text.insert(tk.END, f"The database might be distorted")
     else:
         main_db_name_result_var.set('NOT SET')
         main_db_name_blocker = 0
 
 
@@ -326,155 +384,199 @@
     if db_path_blocker == 1 and main_db_name_blocker == 1:
         try:
             dbname = main_db_name_var.get().strip()
             keysDB = dbname[:-3] + 'Keys.db'
             dbnameKeysWindows = '\\' + keysDB
             dbnameKeysUnix = '/' + keysDB
             conn_path_keys = os.path.join(usable_real_path, keysDB)
-            if db_already_exists_blocker == 1 :
-                if os.path.isfile(usable_real_path + dbnameKeysWindows) or os.path.isfile(usable_real_path + dbnameKeysUnix):
+            if db_already_exists_blocker == 1:
+                if os.path.isfile(
+                        usable_real_path +
+                        dbnameKeysWindows) or os.path.isfile(
+                        usable_real_path +
+                        dbnameKeysUnix):
                     keys_db_conn = AD.Database(conn_path_keys)
                     keys_db_conn.addtable()
-                    db_display_text.insert(tk.END, f"Connected to '{keysDB}' ..\n\n")
+                    db_display_text.insert(
+                        tk.END, f"Connected to '{keysDB}' ..\n\n")
                     success_keysdb_connection_blocker = 1
                 else:
                     keys_db_conn = AD.Database(conn_path_keys)
                     keys_db_conn.addtable()
-                    db_display_text.insert(tk.END, f"'{keysDB}' NOT FOUND ! ==> Created and Connected to '{keysDB}' ..\n\n")
+                    db_display_text.insert(
+                        tk.END, f"'{keysDB}' NOT FOUND ! ==> Created and Connected to '{keysDB}' ..\n\n")
                     success_keysdb_connection_blocker = 1
             else:
                 keys_db_conn = AD.Database(conn_path_keys)
                 keys_db_conn.addtable()
-                db_display_text.insert(tk.END, f"Created and Connected to '{keysDB}' ..\n\n")
+                db_display_text.insert(
+                    tk.END, f"Created and Connected to '{keysDB}' ..\n\n")
                 success_keysdb_connection_blocker = 1
-        except:
+        except BaseException:
             db_display_text.delete('1.0', tk.END)
-            db_display_text.insert(tk.END, f"The database might be distorted\n")
+            db_display_text.insert(
+                tk.END, f"The database might be distorted\n")
 
 
 success_maindb_connection_blocker = 0
 success_keysdb_connection_blocker = 0
 db_enable_blocker = 0
+
+
 def path_name_wrapper():
     set_db_path()
     main_db_name()
     keyDBsetup()
-    global db_enable_blocker,success_keysdb_connection_blocker,success_keysdb_connection_blocker
+    global db_enable_blocker, success_keysdb_connection_blocker, success_keysdb_connection_blocker
     if success_keysdb_connection_blocker and success_keysdb_connection_blocker:
         db_enable_blocker = 1
         swich_db_toggle.state(['!disabled'])
     else:
         db_enable_blocker = 0
         swich_db_toggle.state(['disabled'])
 
 
-
-
-
 db_path_var = tk.StringVar()
-db_path_entry = tk.Entry(master=lowerFrame ,
-                        width=31,
-                        font='Calibre 14 bold',
-                        textvariable=db_path_var).place(relx=0.03, rely=0.005)
+db_path_entry = tk.Entry(master=lowerFrame,
+                         width=31,
+                         font='Calibre 14 bold',
+                         textvariable=db_path_var).place(relx=0.03, rely=0.005)
 
 db_path_result_var = tk.StringVar(value="")
-db_path_result_entry = tk.Label(master=lowerFrame ,
-                        font='Calibre 13 bold',
-                        bootstyle='light',
-                        textvariable=db_path_result_var).place(relx=0.7, rely=0.022)
-
-path_label = tk.Label(master=lowerFrame ,
-                        font='Calibre 13 bold',
-                        bootstyle='light',
-                        text='DATABASES PATH').place(relx=0.47, rely=0.022)
-
-main_database_label = tk.Label(master=lowerFrame ,
-                        font='Calibre 13 bold',
-                        bootstyle='light',
-                        text='MAIN DATABASE').place(relx=0.47, rely=0.205)
+db_path_result_entry = tk.Label(
+    master=lowerFrame,
+    font='Calibre 13 bold',
+    bootstyle='light',
+    textvariable=db_path_result_var).place(
+        relx=0.7,
+    rely=0.022)
+
+path_label = tk.Label(master=lowerFrame,
+                      font='Calibre 13 bold',
+                      bootstyle='light',
+                      text='DATABASES PATH').place(relx=0.47, rely=0.022)
+
+main_database_label = tk.Label(
+    master=lowerFrame,
+    font='Calibre 13 bold',
+    bootstyle='light',
+    text='MAIN DATABASE').place(
+        relx=0.47,
+    rely=0.205)
+
+set_db_path_button = tk.Button(
+    master=lowerFrame,
+    text='SUBMIT PATH AND NAME',
+    width=49,
+    command=path_name_wrapper,
+    bootstyle='info outline')
+set_db_path_button.place(relx=0.031, rely=0.38)
 
-set_db_path_button = tk.Button(master=lowerFrame , text='SUBMIT PATH AND NAME',width=49 ,command=path_name_wrapper,bootstyle='info outline')
-set_db_path_button.place(relx=0.031,rely=0.38)
 
 def checksize():
-    global db_enable_blocker,main_db_conn,keys_db_conn
+    global db_enable_blocker, main_db_conn, keys_db_conn
     if db_enable_blocker != 0:
         if swich_db_var.get() == 1:
             conn = keys_db_conn
         else:
             conn = main_db_conn
         size = conn.size
         if size < 1024:
             db_display_text.delete('1.0', tk.END)
-            db_display_text.insert(tk.END, f"Current size is {size:.5f} (MB)'\n\n")
+            db_display_text.insert(
+                tk.END, f"Current size is {size:.5f} (MB)'\n\n")
         if size >= 1024:
             db_display_text.delete('1.0', tk.END)
-            db_display_text.insert(tk.END, f"Current size is {(size/1024):.3f} (GB)'\n\n")
+            db_display_text.insert(
+                tk.END, f"Current size is {(size/1024):.3f} (GB)'\n\n")
 
 
+size_button = tk.Button(
+    master=lowerFrame,
+    text='SIZE',
+    width=22,
+    command=checksize,
+    bootstyle='warning outline')
+size_button.place(relx=0.031, rely=0.58)
 
-size_button = tk.Button(master=lowerFrame , text='SIZE',width=22 ,command=checksize,bootstyle='warning outline')
-size_button.place(relx=0.031,rely=0.58)
 
 def checkid():
-    global db_enable_blocker,main_db_conn,keys_db_conn
+    global db_enable_blocker, main_db_conn, keys_db_conn
     if db_enable_blocker != 0:
         if swich_db_var.get() == 1:
             conn = keys_db_conn
         else:
             conn = main_db_conn
         try:
             q = conn.query('SELECT ID FROM Classified')
             idd = 0
             for e in q:
                 for k, v in e.items():
                     idd += v[-1][-1][0]
             db_display_text.delete('1.0', tk.END)
             db_display_text.insert(tk.END, f"Last inserted ID is : '{idd}'\n")
-            return(idd)
-        except:
+            return (idd)
+        except BaseException:
             db_display_text.delete('1.0', tk.END)
             db_display_text.insert(tk.END, f"Last inserted ID is : '0'\n")
             return (-1)
 
 
+id_button = tk.Button(
+    master=lowerFrame,
+    text='LAST ID',
+    width=22,
+    command=checkid,
+    bootstyle='warning outline')
+id_button.place(relx=0.247, rely=0.58)
 
 
-id_button = tk.Button(master=lowerFrame , text='LAST ID',width=22 ,command=checkid,bootstyle='warning outline')
-id_button.place(relx=0.247,rely=0.58)
-
 def check_las_mod():
-    global db_enable_blocker,main_db_conn,keys_db_conn
+    global db_enable_blocker, main_db_conn, keys_db_conn
     if db_enable_blocker != 0:
         if swich_db_var.get() == 1:
             conn = keys_db_conn
         else:
             conn = main_db_conn
         db_display_text.delete('1.0', tk.END)
-        db_display_text.insert(tk.END, f"Last modification at : '{conn.last_mod}'\n")
+        db_display_text.insert(
+            tk.END, f"Last modification at : '{conn.last_mod}'\n")
 
 
-las_mod_button = tk.Button(master=lowerFrame , text='LAST MODIFICATION',width=49 ,command=check_las_mod,bootstyle='warning outline')
-las_mod_button.place(relx=0.031,rely=0.74)
+las_mod_button = tk.Button(
+    master=lowerFrame,
+    text='LAST MODIFICATION',
+    width=49,
+    command=check_las_mod,
+    bootstyle='warning outline')
+las_mod_button.place(relx=0.031, rely=0.74)
 
 
 main_db_name_var = tk.StringVar()
-main_db_name_entry = tk.Entry(master=lowerFrame ,
-                        width=31,
-                        font='Calibre 14 bold',
-                        textvariable=main_db_name_var).place(relx=0.03, rely=0.192)
+main_db_name_entry = tk.Entry(
+    master=lowerFrame,
+    width=31,
+    font='Calibre 14 bold',
+    textvariable=main_db_name_var).place(
+        relx=0.03,
+    rely=0.192)
 
 
 main_db_name_result_var = tk.StringVar(value='')
-main_db_name_result_entry = tk.Label(master=lowerFrame ,
-                        font='Calibre 13 bold',
-                        bootstyle='light',
-                        textvariable=main_db_name_result_var).place(relx=0.7, rely=0.205)
+main_db_name_result_entry = tk.Label(
+    master=lowerFrame,
+    font='Calibre 13 bold',
+    bootstyle='light',
+    textvariable=main_db_name_result_var).place(
+        relx=0.7,
+    rely=0.205)
 
 current_working_db = maindbname
+
+
 def swich_db():
     global current_working_db
     if db_enable_blocker != 0:
         if swich_db_var.get() == 1:
             switch_db_label_var.set('ON KEYS')
             db_display_text.delete('1.0', tk.END)
             db_display_text.insert(tk.END, f"Switched to keys database\n")
@@ -483,440 +585,525 @@
             switch_db_label_var.set('ON MAIN')
             db_display_text.delete('1.0', tk.END)
             db_display_text.insert(tk.END, f"Back to default main database\n")
             current_working_db = maindbname[:-3] + 'Keys.db'
 
 
 switch_db_label_var = tk.StringVar(value='SWITCH DATABASE')
-switch_db_label =  tk.Label(master=lowerFrame,
-                            textvariable=switch_db_label_var,
-                            bootstyle = 'light',
-                            font='Calibre 13 bold').place(relx=0.52,rely=0.39)
-
+switch_db_label = tk.Label(master=lowerFrame,
+                           textvariable=switch_db_label_var,
+                           bootstyle='light',
+                           font='Calibre 13 bold').place(relx=0.52, rely=0.39)
 
 
 swich_db_var = tk.IntVar(value=0)
 swich_db_toggle = tk.Checkbutton(bootstyle='light,squared-toggle',
-                        master=lowerFrame,
-                        variable=swich_db_var,
-                        offvalue=0,
-                        onvalue=1,
-                        command=swich_db)
+                                 master=lowerFrame,
+                                 variable=swich_db_var,
+                                 offvalue=0,
+                                 onvalue=1,
+                                 command=swich_db)
 swich_db_toggle.state(['disabled'])
 
 
-
-
-swich_db_toggle.place(relx=0.47,rely=0.413)
+swich_db_toggle.place(relx=0.47, rely=0.413)
 
 
 '''-------------------------------TEXT DECRYPTION/ENCRYPTION STARTED---------------------------------------------------'''
 
 
 def encryption():
     m = inputfield1_1.get()
-    if AF.CryptFile.keyverify(mainkeyvar.get()) == 1 and keySelectionFlag.get() == 1:
-        if len(m) > 200 :
+    if AF.CryptFile.keyverify(
+            mainkeyvar.get()) == 1 and keySelectionFlag.get() == 1:
+        if len(m) > 200:
             outputvar1.set('Too Long')
-        else :
+        else:
             if inputfield1_1.get():
                 progressbar.start()
                 a = AT.Crypt(m, mainkeyvar.get())
-                b =  a.encrypt()[1]
+                b = a.encrypt()[1]
                 outputvar1.set(b.__str__())
                 if var1.get() == 1:
                     qr.tqr(b)
 
 
 def decryption():
-    n =inputfield2_1.get()
-    if AF.CryptFile.keyverify(mainkeyvar.get()) == 1 and keySelectionFlag.get() == 1:
+    n = inputfield2_1.get()
+    if AF.CryptFile.keyverify(
+            mainkeyvar.get()) == 1 and keySelectionFlag.get() == 1:
         if inputfield2_1.get():
             progressbar2.start()
             a = AT.Crypt(n, mainkeyvar.get())
             b = a.decrypt()[1]
             outputvar2.set(b.__str__())
             if var2.get() == 1:
                 if not len(b) > 200:
                     qr.tqr(b)
 
+
 def func1():
-    if var1.get() == 1 :
+    if var1.get() == 1:
         label1.config(text='QR ON')
     else:
         label1.config(text='QR OFF')
 
+
 def func2():
-    if var2.get() == 1 :
+    if var2.get() == 1:
         label2.config(text='QR ON')
     else:
         label2.config(text='QR OFF')
 
 
-button1 = tk.Button(master=textFrame1 ,text='ENCRYPT', command=encryption, bootstyle='light outline').place(relx=0.42, rely=0.73)
-button2 = tk.Button(master=textFrame2 , text='DECRYPT', command=decryption,bootstyle='light outline').place(relx=0.42,rely=0.8)
+button1 = tk.Button(
+    master=textFrame1,
+    text='ENCRYPT',
+    command=encryption,
+    bootstyle='light outline').place(
+        relx=0.42,
+    rely=0.73)
+button2 = tk.Button(
+    master=textFrame2,
+    text='DECRYPT',
+    command=decryption,
+    bootstyle='light outline').place(
+        relx=0.42,
+    rely=0.8)
 
 inputfield1_1 = tk.StringVar()
-textfield1_1 = tk.Entry(master=textFrame1 ,
+textfield1_1 = tk.Entry(master=textFrame1,
                         width=20,
                         font='Calibre 11 bold',
-                        textvariable=inputfield1_1).place(relx=0.29 , rely=0.30)
+                        textvariable=inputfield1_1).place(relx=0.29, rely=0.30)
 
 inputfield2_1 = tk.StringVar(value='')
-textfield2_1 = tk.Entry(master=textFrame2 ,
-                        font='Calibre 11 bold',
-                        width=20,
-                        textvariable=inputfield2_1).place(relx=0.290 ,rely=0.38)
+textfield2_1 = tk.Entry(
+    master=textFrame2,
+    font='Calibre 11 bold',
+    width=20,
+    textvariable=inputfield2_1).place(
+        relx=0.290,
+    rely=0.38)
 
-namelabel1 = tk.Label(master=textFrame1 ,
+namelabel1 = tk.Label(master=textFrame1,
                       text='TEXT ENCRYPTION',
-                      font='Calibre 20 bold' ,
+                      font='Calibre 20 bold',
                       )
-namelabel1.place(relx=0.190 ,rely=0.10)
-namelabel2 = tk.Label(master=textFrame2 ,
-                      text='TEXT DECRYPTION' ,
-                      font='Calibre 20 bold'  ,
-                      ).place(relx=0.190 ,rely=0.200)
+namelabel1.place(relx=0.190, rely=0.10)
+namelabel2 = tk.Label(master=textFrame2,
+                      text='TEXT DECRYPTION',
+                      font='Calibre 20 bold',
+                      ).place(relx=0.190, rely=0.200)
 
 outputvar1 = tk.StringVar(value='')
-outputlabel1 =  tk.Entry(master= textFrame1,
-                         textvariable=outputvar1,
-                         font='terminal 11 bold').place(relx= 0.02,
-                                                       rely= 0.48 ,
-                                                       width= 480,
-                                                       height= 50)
+outputlabel1 = tk.Entry(master=textFrame1,
+                        textvariable=outputvar1,
+                        font='terminal 11 bold').place(relx=0.02,
+                                                       rely=0.48,
+                                                       width=480,
+                                                       height=50)
 outputvar2 = tk.StringVar(value='')
-outputlabel2 = tk.Entry(master=textFrame2 ,
-                        textvariable= outputvar2 ,
-                        font='terminal 11 bold').place(relx= 0.02,
-                                                       rely= 0.55,
-                                                       width= 480,
-                                                       height= 50)
-
+outputlabel2 = tk.Entry(master=textFrame2,
+                        textvariable=outputvar2,
+                        font='terminal 11 bold').place(relx=0.02,
+                                                       rely=0.55,
+                                                       width=480,
+                                                       height=50)
 
 
-label1 = tk.Label(master=textFrame1,text='QR',font=('terminal',17))
-label1.place(relx=0.2,rely=0.75)
+label1 = tk.Label(master=textFrame1, text='QR', font=('terminal', 17))
+label1.place(relx=0.2, rely=0.75)
 var1 = tk.IntVar()
 mytoolbutt3 = tk.Checkbutton(bootstyle='success , round-toggle',
-                        master=textFrame1,
-                        variable=var1,
-                        offvalue=0,
-                        command=func1)
-
-mytoolbutt3.place(relx=0.1,rely=0.77)
+                             master=textFrame1,
+                             variable=var1,
+                             offvalue=0,
+                             command=func1)
 
+mytoolbutt3.place(relx=0.1, rely=0.77)
 
 
-
-label2 = tk.Label(master=textFrame2,text='QR',font=('terminal',17))
-label2.place(relx=0.2,rely=0.82)
+label2 = tk.Label(master=textFrame2, text='QR', font=('terminal', 17))
+label2.place(relx=0.2, rely=0.82)
 var2 = tk.IntVar()
 mytoolbutt6 = tk.Checkbutton(bootstyle='success , round-toggle',
-                        master=textFrame2,
-                        variable=var2,
-                        offvalue=0,
-                        command=func2)
-
-mytoolbutt6.place(relx=0.1,rely=0.84)
-
-
-progressbar = tk.Progressbar(master=textFrame1,mode='indeterminate',style='secondary',length=100,)
-progressbar.place(relx=0.05,rely=0.34)
-
-progressbar2 = tk.Progressbar(master=textFrame2,mode='indeterminate',style='secondary',length=100,)
-progressbar2.place(relx=0.05,rely=0.42)
+                             master=textFrame2,
+                             variable=var2,
+                             offvalue=0,
+                             command=func2)
+
+mytoolbutt6.place(relx=0.1, rely=0.84)
+
+
+progressbar = tk.Progressbar(
+    master=textFrame1,
+    mode='indeterminate',
+    style='secondary',
+    length=100,
+)
+progressbar.place(relx=0.05, rely=0.34)
+
+progressbar2 = tk.Progressbar(
+    master=textFrame2,
+    mode='indeterminate',
+    style='secondary',
+    length=100,
+)
+progressbar2.place(relx=0.05, rely=0.42)
 
 
 '''-------------------------------FILE ENCRYPTION/DECRYPTION STARTED--------------------------------------------'''
 
 
-filepathlabel = tk.Label(master=frameFile1 ,
-                      text='FILE PATH',
-                      font='Calibre 20 bold' ,
-                      )
-filepathlabel.place(relx=0.335,rely=0.10)
+filepathlabel = tk.Label(master=frameFile1,
+                         text='FILE PATH',
+                         font='Calibre 20 bold',
+                         )
+filepathlabel.place(relx=0.335, rely=0.10)
 
-import platform
 if platform.system() == 'Windows':
     resultvarfile = tk.StringVar(value='                 ..........')
-    resultLabelfile =  tk.Label(master= frameFile1,
-                             textvariable=resultvarfile,
-                             font='terminal 13 bold').place(rely= 0.55)
+    resultLabelfile = tk.Label(master=frameFile1,
+                               textvariable=resultvarfile,
+                               font='terminal 13 bold').place(rely=0.55)
 else:
     resultvarfile = tk.StringVar(value='                    ..........')
     resultLabelfile = tk.Label(master=frameFile1,
                                textvariable=resultvarfile,
                                font='terminal 13 bold').place(rely=0.55)
 
 
 def encFile():
-    global fileaccessSemo ,add_enc_to_db ,main_db_conn,mainkey
-    if 1 :
+    global fileaccessSemo, add_enc_to_db, main_db_conn, mainkey
+    if 1:
         if keySelectionFlag.get() != 0:
             filename = filenameStringVar.get().strip()
             key = mainkey
             target = AF.CryptFile(filename, key)
             a = target.encrypt()
             if a == 1:
                 filename = filename + '.crypt'
                 filenameStringVar.set(filename)
-                resultvarfile.set('      Encrypted Successfully / added .crypt')
+                resultvarfile.set(
+                    '      Encrypted Successfully / added .crypt')
                 if encfiletoolbuttvar.get() == 1:
-                    with open(filename,'rb') as f:
+                    with open(filename, 'rb') as f:
                         file_content = f.read()
                     try:
-                        main_db_conn.insert(filename,file_content, outputKeyref.get().strip())
-                    except:
+                        main_db_conn.insert(
+                            filename, file_content, outputKeyref.get().strip())
+                    except BaseException:
                         db_display_text.delete('1.0', tk.END)
-                        db_display_text.insert(tk.END, f"ERROR \n\nDatabase might be distorted\n")
+                        db_display_text.insert(
+                            tk.END, f"ERROR \n\nDatabase might be distorted\n")
             if platform.system() == 'Windows':
                 if a == 2:
                     resultvarfile.set('                 File is Empty')
                 if a == 3:
                     resultvarfile.set("               File Doesn't Exist")
                 if a == 0:
                     resultvarfile.set("                  Can't Encrypt")
-                if  a == 4:
+                if a == 4:
                     resultvarfile.set('                     ERROR')
-                if a == 5 :
+                if a == 5:
                     resultvarfile.set('          ERROR : Key is Not 512-bit')
                 if a == 6:
-                    resultvarfile.set('       ERROR : File is already encrypted')
+                    resultvarfile.set(
+                        '       ERROR : File is already encrypted')
                 elif a == 7:
-                    resultvarfile.set(' ERROR : Given a directory instead of a file')
+                    resultvarfile.set(
+                        ' ERROR : Given a directory instead of a file')
             else:
                 if a == 2:
                     resultvarfile.set('                   File is Empty')
                 if a == 3:
                     resultvarfile.set("                 File Doesn't Exist")
                 if a == 0:
                     resultvarfile.set("                    Can't Encrypt")
-                if  a == 4:
+                if a == 4:
                     resultvarfile.set('                       ERROR')
-                if a == 5 :
+                if a == 5:
                     resultvarfile.set('            ERROR : Key is Not 512-bit')
                 if a == 6:
-                    resultvarfile.set('         ERROR : File is already encrypted')
+                    resultvarfile.set(
+                        '         ERROR : File is already encrypted')
                 elif a == 7:
-                    resultvarfile.set('   ERROR : Given a directory instead of a file')
+                    resultvarfile.set(
+                        '   ERROR : Given a directory instead of a file')
+
 
 def decfile():
-    global fileaccessSemo,add_dec_to_db,main_db_conn,mainkey
+    global fileaccessSemo, add_dec_to_db, main_db_conn, mainkey
     if 1:
         if keySelectionFlag.get() != 0:
-            filename =filenameStringVar.get().strip()
+            filename = filenameStringVar.get().strip()
             key = mainkey
             target = AF.CryptFile(filename, key)
             a = target.decrypt()
             if a == 1:
                 filename = os.path.splitext(filename)[0]
                 filenameStringVar.set(filename)
-                resultvarfile.set('     Decrypted Successfully + removed .crypt')
+                resultvarfile.set(
+                    '     Decrypted Successfully + removed .crypt')
                 if decfiletoolbuttvar.get() == 1:
-                    with open(filename,'rb') as f:
+                    with open(filename, 'rb') as f:
                         file_content = f.read()
                     try:
-                        main_db_conn.insert(filename,file_content, outputKeyref.get().strip())
-                    except:
+                        main_db_conn.insert(
+                            filename, file_content, outputKeyref.get().strip())
+                    except BaseException:
                         db_display_text.delete('1.0', tk.END)
-                        db_display_text.insert(tk.END, f"ERROR \n\nDatabase might be distorted\n")
+                        db_display_text.insert(
+                            tk.END, f"ERROR \n\nDatabase might be distorted\n")
             if platform.system() == 'Windows':
                 if a == 2:
                     resultvarfile.set('                 File is Empty')
                 if a == 3:
                     resultvarfile.set("               File Doesn't Exist")
                 if a == 0:
                     resultvarfile.set("                 Can't Decrypt")
-                if  a == 4:
+                if a == 4:
                     resultvarfile.set('                     ERROR')
-                elif a == 5 :
+                elif a == 5:
                     resultvarfile.set('          ERROR : Key is Not 512-bit')
                 if a == 6:
-                    resultvarfile.set('       ERROR : File is already decrypted')
+                    resultvarfile.set(
+                        '       ERROR : File is already decrypted')
                 elif a == 7:
-                    resultvarfile.set(' ERROR : Given a directory instead of a file')
+                    resultvarfile.set(
+                        ' ERROR : Given a directory instead of a file')
             else:
                 if a == 2:
                     resultvarfile.set('                   File is Empty')
                 if a == 3:
                     resultvarfile.set("                 File Doesn't Exist")
                 if a == 0:
                     resultvarfile.set("                   Can't Decrypt")
-                if  a == 4:
+                if a == 4:
                     resultvarfile.set('                       ERROR')
-                elif a == 5 :
+                elif a == 5:
                     resultvarfile.set('            ERROR : Key is Not 512-bit')
                 if a == 6:
-                    resultvarfile.set('         ERROR : File is already decrypted')
+                    resultvarfile.set(
+                        '         ERROR : File is already decrypted')
                 elif a == 7:
-                    resultvarfile.set('   ERROR : Given a directory instead of a file')
-
-
+                    resultvarfile.set(
+                        '   ERROR : Given a directory instead of a file')
 
 
-
-
-
-
-encryptionfilebutton = tk.Button(master=frameFile1 ,text='ENCRYPT FILE', command=encFile, bootstyle='warning outline').place(relx=0.25, rely=0.73)
-decryptionfilebutton = tk.Button(master=frameFile1 , text='DECRYPT FILE', command=decfile,bootstyle='warning outline').place(relx=0.55,rely=0.73)
+encryptionfilebutton = tk.Button(
+    master=frameFile1,
+    text='ENCRYPT FILE',
+    command=encFile,
+    bootstyle='warning outline').place(
+        relx=0.25,
+    rely=0.73)
+decryptionfilebutton = tk.Button(
+    master=frameFile1,
+    text='DECRYPT FILE',
+    command=decfile,
+    bootstyle='warning outline').place(
+        relx=0.55,
+    rely=0.73)
 
 filenameStringVar = tk.StringVar(value='')
 
-filenametext = tk.Entry(master=frameFile1 ,
-                        width=31,
-                        font='Calibre 15 bold',
-                        textvariable=filenameStringVar).place(relx=0.05, rely=0.30)
-
+filenametext = tk.Entry(
+    master=frameFile1,
+    width=31,
+    font='Calibre 15 bold',
+    textvariable=filenameStringVar).place(
+        relx=0.05,
+    rely=0.30)
+
+
+addtodbLabel = tk.Label(
+    master=frameFile1,
+    text='ADD TO DATABASE',
+    font=(
+        'Calibre',
+        11),
+    bootstyle='warning')
+addtodbLabel.place(relx=0.35, rely=0.908)
 
+add_enc_to_db = 0
 
-addtodbLabel = tk.Label(master=frameFile1,text='ADD TO DATABASE',font=('Calibre',11),bootstyle='warning')
-addtodbLabel.place(relx=0.35,rely=0.908)
 
-add_enc_to_db = 0
 def encToggleButtFunc():
     global add_enc_to_db
     if encfiletoolbuttvar == 1:
         add_enc_to_db = 1
     else:
         add_enc_to_db = 0
 
+
 add_dec_to_db = 0
+
+
 def decToggleButtFunc():
     global add_dec_to_db
     if decfiletoolbuttvar == 1:
         add_dec_to_db = 1
     else:
         add_dec_to_db = 0
 
+
 encfiletoolbuttvar = tk.IntVar()
 encfiletoolbutt = tk.Checkbutton(bootstyle='warning , round-toggle',
-                        master=frameFile1,
-                        variable=encfiletoolbuttvar,
-                        offvalue=0,
-                        onvalue=1,
-                        command=encToggleButtFunc)
+                                 master=frameFile1,
+                                 variable=encfiletoolbuttvar,
+                                 offvalue=0,
+                                 onvalue=1,
+                                 command=encToggleButtFunc)
 encfiletoolbutt.state(['disabled'])
-encfiletoolbutt.place(relx=0.25,rely=0.92)
+encfiletoolbutt.place(relx=0.25, rely=0.92)
 
 
 decfiletoolbuttvar = tk.IntVar()
 decfiletoolbutt = tk.Checkbutton(bootstyle='warning , round-toggle',
-                        master=frameFile1,
-                        variable=decfiletoolbuttvar,
-                        offvalue=0,
-                        command=decToggleButtFunc)
+                                 master=frameFile1,
+                                 variable=decfiletoolbuttvar,
+                                 offvalue=0,
+                                 command=decToggleButtFunc)
 decfiletoolbutt.state(['disabled'])
-decfiletoolbutt.place(relx=0.717,rely=0.92)
+decfiletoolbutt.place(relx=0.717, rely=0.92)
 
 
+keySelectionFlag = tk.IntVar(value=0)
 
 
-keySelectionFlag = tk.IntVar(value=0)
 def mainKeyWrapper():
-    global success_keysdb_connection_blocker,mainkey
-    if AF.CryptFile.keyverify(mainkeyvar.get().strip()) == 1 :
+    global success_keysdb_connection_blocker, mainkey
+    if AF.CryptFile.keyverify(mainkeyvar.get().strip()) == 1:
         mainkey = mainkeyvar.get().strip()
         keyrefGen()
         keyselectionvar.set('       SELECTED')
         keySelectionFlag.set(1)
         try:
-            if success_keysdb_connection_blocker and os.path.isfile(filenameStringVar.get().strip()):
-                keys_db_conn.insert(filenameStringVar.get().strip(),mainkey,outputKeyref.get())
-            if success_keysdb_connection_blocker and not os.path.isfile(filenameStringVar.get().strip()):
-                keys_db_conn.insert('STANDALONE',mainkey,outputKeyref.get())
-        except:
+            if success_keysdb_connection_blocker and os.path.isfile(
+                    filenameStringVar.get().strip()):
+                keys_db_conn.insert(
+                    filenameStringVar.get().strip(),
+                    mainkey,
+                    outputKeyref.get())
+            if success_keysdb_connection_blocker and not os.path.isfile(
+                    filenameStringVar.get().strip()):
+                keys_db_conn.insert('STANDALONE', mainkey, outputKeyref.get())
+        except BaseException:
             db_display_text.delete('1.0', tk.END)
             db_display_text.insert(tk.END, f"Faulty Database\n")
-    else :
+    else:
         keySelectionFlag.set(0)
         keyselectionvar.set('     NOT SELECTED')
 
 
-mainkeyLabel = tk.Label(master=frameFile2 ,
-                      text='MAIN KEY' ,
-                      font='Calibre 20 bold',
-                      bootstyle='info',
-                      ).place(relx=0.3 ,rely=0.075)
+mainkeyLabel = tk.Label(master=frameFile2,
+                        text='MAIN KEY',
+                        font='Calibre 20 bold',
+                        bootstyle='info',
+                        ).place(relx=0.3, rely=0.075)
 
 
 mainkeyvar = tk.StringVar()
-mainkeyEntry = tk.Entry(master=frameFile2 ,
+mainkeyEntry = tk.Entry(master=frameFile2,
                         font='Calibre 14 bold',
                         textvariable=mainkeyvar,
                         width=29
-                        ).place(relx=0.09 ,rely=0.29)
+                        ).place(relx=0.09, rely=0.29)
 
 
 def keyrefGen():
     ref = '#'
     for _ in range(6):
-        character = secrets.choice(string.ascii_letters + string.digits + '$' + '?' + '&' + '@' + '!' + '-' + '+')
+        character = secrets.choice(
+            string.ascii_letters +
+            string.digits +
+            '$' +
+            '?' +
+            '&' +
+            '@' +
+            '!' +
+            '-' +
+            '+')
         ref += character
     outputKeyref.set(ref)
 
 
-
 outputKeyref = tk.StringVar(value='#XXXXXX')
-keyrefLabel = tk.Label(master=frameFile2,textvariable=outputKeyref,bootstyle='secondary',font=('terminal',12))
-keyrefLabel.place(relx=0.712,rely=0.12)
-
-keySelectButton = tk.Button(master=frameFile2 ,text='SELECT KEY', command=mainKeyWrapper, bootstyle='info outline').place(relx=0.6725, rely=0.5)
+keyrefLabel = tk.Label(
+    master=frameFile2,
+    textvariable=outputKeyref,
+    bootstyle='secondary',
+    font=(
+        'terminal',
+        12))
+keyrefLabel.place(relx=0.712, rely=0.12)
+
+keySelectButton = tk.Button(
+    master=frameFile2,
+    text='SELECT KEY',
+    command=mainKeyWrapper,
+    bootstyle='info outline').place(
+        relx=0.6725,
+    rely=0.5)
 
 
 keyselectionvar = tk.StringVar(value='   KEY NOT SELECTED')
-keyselectionLabel = tk.Label(master=frameFile2 ,
-                        textvariable= keyselectionvar ,
-                        bootstyle='info',
-                        font='terminal 11 bold').place(relx= 0.15 ,
-                                        rely= 0.465,
-                                        height= 50)
-
+keyselectionLabel = tk.Label(master=frameFile2,
+                             textvariable=keyselectionvar,
+                             bootstyle='info',
+                             font='terminal 11 bold').place(relx=0.15,
+                                                            rely=0.465,
+                                                            height=50)
 
 
 def genMainKey():
     keyGenVar.set(AF.CryptFile.genkey())
 
 
 keyGenVar = tk.StringVar(value='')
-keyGenEntry = tk.Entry(master=frameFile2 ,
-                        font='Calibre 12 bold',
-                        textvariable=keyGenVar,
-                        width=23).place(relx=0.1 ,rely=0.69)
+keyGenEntry = tk.Entry(master=frameFile2,
+                       font='Calibre 12 bold',
+                       textvariable=keyGenVar,
+                       width=23).place(relx=0.1, rely=0.69)
 
-keyButton = tk.Button(master=frameFile2 ,
+keyButton = tk.Button(master=frameFile2,
                       text='GENERATE',
                       command=genMainKey,
                       bootstyle='success outline').place(relx=0.671, rely=0.7)
 
 
 '''---------------------------------------STAMP STARTED -------------------------------------------------------'''
 
 
-latest_ID_key_label = tk.Label(master=lowerFrame,text='GitHub.com/AshGw/AES-256', font='Calibre 6')
-latest_ID_key_label.place(relx=0.84,rely=0.92)
+latest_ID_key_label = tk.Label(
+    master=lowerFrame,
+    text='GitHub.com/AshGw/AES-256',
+    font='Calibre 6')
+latest_ID_key_label.place(relx=0.84, rely=0.92)
 
 '''---------------------------------------STAMP ENDED-------------------------------------------------------'''
 
+
 def rm_json():
     global usable_real_path
-    file = os.path.join(usable_real_path,'output.json')
+    file = os.path.join(usable_real_path, 'output.json')
     if os.path.exists(file):
         os.remove(file)
 
+
 def rm_qr():
     if os.path.exists('qrv10.png'):
         os.remove('qrv10.png')
 
+
 def rm_all():
     rm_qr()
     rm_json()
 
-atexit.register(rm_all)
 
+atexit.register(rm_all)
 
 
 if __name__ == '__main__':
     object.mainloop()
-
-
```

### Comparing `AshCrypt-1.3.4/AshCrypt/CliCrypt.py` & `AshCrypt-1.3.5/AshCrypt/CliCrypt.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,86 +6,93 @@
 
 print('Welcome to the CLI')
 
 commands = 'Commands : \n\tq: to quit the program \n\tc : view commands\n\te: for encryption\n\td : for decryption\n' \
            '\tef : to encrypt a file\n\tdf : to decrypt a file\n'
 
 global key
-def input_selection(q=None,c=None,e=None,d=None,ef=None,df=None):
-    global encflag,decFlag,file_decFlag,file_encFlag
-    if q == 1 :
+
+
+def input_selection(q=None, c=None, e=None, d=None, ef=None, df=None):
+    global encflag, decFlag, file_decFlag, file_encFlag
+    if q == 1:
         sys.exit()
-    if c == 1 :
+    if c == 1:
         print(commands)
-    if e == 1 :
+    if e == 1:
         file_decFlag = False
         file_encFlag = False
         decFlag = False
         encflag = True
         enc()
-    if d == 1 :
+    if d == 1:
         file_decFlag = False
         file_encFlag = False
         encflag = False
         decFlag = True
         dec()
-    if ef == 1 :
+    if ef == 1:
         decFlag = False
         encflag = False
         file_decFlag = False
         file_encFlag = True
         file_enc()
-    if df == 1 :
+    if df == 1:
         encflag = False
         decFlag = True
         file_encFlag = False
         file_decFlag = True
         file_dec()
-    else :
+    else:
         pass
 
-def inputWrap(inp) :
-        inp = inp.lower()
-        if inp == 'c':
-            input_selection(c=1)
-            return 'c'
-        if inp == 'q' :
-            input_selection(q=1)
-            return 'q'
-        if inp == 'e' :
-            input_selection(e=1)
-            return 'e'
-        if inp == 'd' :
-            input_selection(d=1)
-            return 'd'
-        if inp == 'ef' :
-            input_selection(ef=1)
-            return 'ef'
-        if inp == 'df' :
-            input_selection(df=1)
-            return 'df'
-        else :
-            return None
+
+def inputWrap(inp):
+    inp = inp.lower()
+    if inp == 'c':
+        input_selection(c=1)
+        return 'c'
+    if inp == 'q':
+        input_selection(q=1)
+        return 'q'
+    if inp == 'e':
+        input_selection(e=1)
+        return 'e'
+    if inp == 'd':
+        input_selection(d=1)
+        return 'd'
+    if inp == 'ef':
+        input_selection(ef=1)
+        return 'ef'
+    if inp == 'df':
+        input_selection(df=1)
+        return 'df'
+    else:
+        return None
+
+
 def intro():
     intro = True
     while intro:
         print('Program started running..')
         print('Press c to view commands : ')
         while True:
             n = input("Press..\n")
             inputWrap(n)
+
+
 def keysetup():
     outer = True
     inner = True
-    while outer :
+    while outer:
         global key
         key = ''
         i = input('Do you have a key ?(y/n) : ')
         inputWrap(i)
-        if i.lower() == 'n' :
+        if i.lower() == 'n':
             print("Here's your key : ")
             key = A.Crypt.genkey()
             print(key)
             inner = False
             outer = False
         elif i.lower() == 'y':
             while inner:
@@ -96,113 +103,127 @@
                     print('Key selected\n')
                     key = kk
                     inner = False
                     outer = False
                 else:
                     print('Enter a valid key !\n')
 
+
 encflag = True
+
+
 def enc():
     keysetup()
     while encflag:
         print()
         global key
         print("press c to view commands.. ")
         message = input('Encrypt a message : ')
         inputWrap(message)
         a = A.Crypt(message, key=key)
         enc = a.encrypt()
         if (enc[0]) == 1:
             print("Success ! Here's the message : ")
-            print('\t',enc[1],'\n')
+            print('\t', enc[1], '\n')
         else:
             print('Error occurred during the encryption process\n')
 
+
 decFlag = True
+
+
 def dec():
     keysetup()
     while decFlag:
         print()
         global key
         print("press c to view commands.. ")
         message = input('Decrypt a message : ')
         inputWrap(message)
         a = A.Crypt(message, key=key)
         dec = a.decrypt()
         if (dec[0]) == 1:
             print("Success ! Here's the message : ")
-            print('\t',dec[1],'\n')
+            print('\t', dec[1], '\n')
         else:
             print('Error occurred during the decryption process\n')
 
+
 file_encFlag = True
 
 
 file_decFlag = True
+
+
 def file_dec():
     keysetup()
-    while file_decFlag :
+    while file_decFlag:
         print()
         global key
-        pre = input("running file decryption mode , press the known commands or 'Enter' to continue.. : ")
+        pre = input(
+            "running file decryption mode , press the known commands or 'Enter' to continue.. : ")
         print()
         inputWrap(pre)
-        if pre == '' :
+        if pre == '':
             print("You can use the commands AFTER entering the file name.. ")
             filename = input('Enter full file name to be Decrypted : ')
             target = AF.CryptFile(filename, key)
             a = target.decrypt()
             if a == 1:
                 print('File successfully decrypted + removed .crypt extension')
                 print(f'File is now named {os.path.splitext(filename)[0]}')
             if a == 2:
                 print('Cannot decrypt the file  when it is already empty')
             if a == 3:
-                print(f'The file named : "{filename}" does not exists , try specifying the whole sys path')
+                print(
+                    f'The file named : "{filename}" does not exists , try specifying the whole sys path')
             if a == 0:
-                print('Error in the decryption process. Check if the the file is distorted or it might just be '
-                      'decrypted already')
-            if a == 4 :
+                print(
+                    'Error in the decryption process. Check if the the file is distorted or it might just be '
+                    'decrypted already')
+            if a == 4:
                 print('Unknown Error has occurred\n')
-            if a == 5 :
+            if a == 5:
                 print('ERROR : Key is Not 512-bit')
             if a == 6:
                 print('ERROR : File is already decrypted')
             elif a == 7:
                 print('ERROR : Given a directory instead of a file')
 
 
 def file_enc():
     keysetup()
-    while file_encFlag :
+    while file_encFlag:
         print()
         global key
-        pre = input("running file encryption mode, press the known commands or 'Enter' to continue.. : ")
+        pre = input(
+            "running file encryption mode, press the known commands or 'Enter' to continue.. : ")
         print()
         inputWrap(pre)
-        if pre == '' :
+        if pre == '':
             print("You can use the commands AFTER entering the file name.. ")
             filename = input('Enter full file name to be Encrypted : ')
             target = AF.CryptFile(filename, key)
             a = target.encrypt()
             if a == 1:
                 print('File successfully encrypted + added .crypt extension')
                 print(f"File is now named : '{filename}.crypt' ")
             if a == 2:
                 print('Cannot encrypt the file  when it is already empty')
             if a == 3:
-                print(f'The file named : "{filename}" does not exists , try specifying the whole sys path')
+                print(
+                    f'The file named : "{filename}" does not exists , try specifying the whole sys path')
             if a == 0:
-                print('Error in the encryption process. Check if the the file is distorted')
-            elif a == 4 :
+                print(
+                    'Error in the encryption process. Check if the the file is distorted')
+            elif a == 4:
                 print('Unknown Error has occurred\n')
-            if a == 5 :
+            if a == 5:
                 print('ERROR : Key is Not 512-bit')
             if a == 6:
                 print('ERROR : File is already encrypted')
             elif a == 7:
                 print('ERROR : Given a directory instead of a file')
 
 
-
 if __name__ == '__main__':
-    intro()
+    intro()
```

### Comparing `AshCrypt-1.3.4/AshCrypt/Database.py` & `AshCrypt-1.3.5/AshCrypt/Database.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
-from dataclasses import dataclass,field
+from dataclasses import dataclass, field
 from datetime import datetime
 from typing import Union
 import sqlite3
 import os
 
+
 @dataclass
 class Database():
     dbname: str = field()
     tablename: str = field(default='Classified')
     conn: sqlite3.Connection = field(init=False, repr=False)
     c: sqlite3.Cursor = field(init=False, repr=False)
 
@@ -15,15 +16,16 @@
         self.conn = sqlite3.connect(self.dbname)
         self.c = self.conn.cursor()
 
     @property
     def size(self):         # Size in MB #
         try:
             with self.conn:
-                self.c.execute('SELECT page_count * page_size FROM pragma_page_count() , pragma_page_size')
+                self.c.execute(
+                    'SELECT page_count * page_size FROM pragma_page_count() , pragma_page_size')
                 size_info = self.c.fetchone()
                 size = size_info[0] / 1024 / 1024
                 return size
         except sqlite3.Error as e:
             return (0, e)
 
     @property
@@ -44,82 +46,102 @@
         for i, query in enumerate(querys):
             if not isinstance(query, str):
                 result.append({f'query {i}': (0.0, TypeError)})
             try:
                 with self.conn:
                     self.c.execute(query)
                     if self.c.rowcount == 1:
-                        result.append({f'query {i}': ['SUCCESS',self.c.fetchone()]})
+                        result.append(
+                            {f'query {i}': ['SUCCESS', self.c.fetchone()]})
                     else:
-                        result.append({f'query {i}': ['SUCCESS',self.c.fetchall()]})
+                        result.append(
+                            {f'query {i}': ['SUCCESS', self.c.fetchall()]})
 
             except sqlite3.Error as e:
                 result.append({f'query {i}': ('FAILURE', e.__str__())})
         return result
 
     def addtable(self, optional_tablename=None):
         if optional_tablename is None:
             try:
                 with self.conn:
-                    self.c.execute(f"CREATE TABLE IF NOT EXISTS {self.tablename} "
-                                   "(ID INTEGER PRIMARY KEY, Name Text , Content BLOB ,Key TEXT )")
+                    self.c.execute(
+                        f"CREATE TABLE IF NOT EXISTS {self.tablename} "
+                        "(ID INTEGER PRIMARY KEY, Name Text , Content BLOB ,Key TEXT )")
                 return 11
             except sqlite3.Error as e:
                 return (0.0, e)
 
         else:
             try:
                 with self.conn:
-                    self.c.execute(f"CREATE TABLE IF NOT EXISTS {optional_tablename} "
-                                   "(ID INTEGER PRIMARY KEY,"
-                                   "Name TEXT ,"
-                                   "Content BLOB ,"
-                                   "Key TEXT )")
+                    self.c.execute(
+                        f"CREATE TABLE IF NOT EXISTS {optional_tablename} "
+                        "(ID INTEGER PRIMARY KEY,"
+                        "Name TEXT ,"
+                        "Content BLOB ,"
+                        "Key TEXT )")
                     self.tablename = optional_tablename
                 return 1
 
             except sqlite3.Error as e:
                 return (0, e)
 
-    def insert(self, name , content, key, optional_table_name=None):
+    def insert(self, name, content, key, optional_table_name=None):
         if optional_table_name is None:
             try:
                 with self.conn:
-                    self.c.execute(f"INSERT INTO {self.tablename} (Name , Content ,Key) VALUES (? , ? , ?) "
-                                   , (name,content,key))
+                    self.c.execute(
+                        f"INSERT INTO {self.tablename} (Name , Content ,Key) VALUES (? , ? , ?) ",
+                        (name,
+                         content,
+                         key))
 
                 return 11
             except sqlite3.Error as e:
                 return (0.0, e)
 
         else:
             try:
                 with self.conn:
-                    self.c.execute(f"INSERT INTO {optional_table_name} (Name, Content ,Key) VALUES (? , ? , ?) ",
-                                   (name,content,key))
+                    self.c.execute(
+                        f"INSERT INTO {optional_table_name} (Name, Content ,Key) VALUES (? , ? , ?) ",
+                        (name,
+                         content,
+                         key))
                 return 1
             except sqlite3.Error as e:
                 return (0, e)
 
-    def update(self, column_name: str, new_column_val: str, ID: int, optional_table_name=None):
+    def update(
+            self,
+            column_name: str,
+            new_column_val: str,
+            ID: int,
+            optional_table_name=None):
         if optional_table_name is None:
             try:
                 with self.conn:
-                    self.c.execute((f'UPDATE {self.tablename} SET {column_name} = ? WHERE ID = ? '),
-                                   (new_column_val, ID))
+                    self.c.execute(
+                        (f'UPDATE {self.tablename} SET {column_name} = ? WHERE ID = ? '),
+                        (new_column_val,
+                         ID))
                     return 11
 
             except sqlite3.Error as e:
                 return (0.0, e)
 
         else:
             try:
                 with self.conn:
-                    self.c.execute((f'UPDATE {optional_table_name} SET ? = ? WHERE ID = ? '),
-                                   (column_name, new_column_val, ID))
+                    self.c.execute(
+                        (f'UPDATE {optional_table_name} SET ? = ? WHERE ID = ? '),
+                        (column_name,
+                         new_column_val,
+                         ID))
                     return 1
 
             except sqlite3.Error as e:
                 return (0, e)
 
     def content(self, optional_tablename=None):
         if optional_tablename is None:
@@ -138,29 +160,31 @@
                     self.c.execute(f'SELECT * FROM {optional_tablename} ')
                     for row in self.c.fetchall():
                         yield row
 
             except sqlite3.Error as e:
                 return (0, e)
 
-    def content_by_id(self, id : int ,optional_tablename=None):
+    def content_by_id(self, id: int, optional_tablename=None):
         if optional_tablename is None:
             try:
                 with self.conn:
-                    self.c.execute(f'SELECT * FROM {self.tablename} WHERE ID = ? ',(id,))
+                    self.c.execute(
+                        f'SELECT * FROM {self.tablename} WHERE ID = ? ', (id,))
                     for row in self.c.fetchall():
                         yield row
 
             except sqlite3.Error as e:
                 return (0.0, e)
 
         else:
             try:
                 with self.conn:
-                    self.c.execute(f'SELECT * FROM {optional_tablename} WHERE ID = ? ',(id,))
+                    self.c.execute(
+                        f'SELECT * FROM {optional_tablename} WHERE ID = ? ', (id,))
                     for row in self.c.fetchall():
                         yield row
 
             except sqlite3.Error as e:
                 return (0, e)
 
     def show_contents(self, *optional_tablenames):
@@ -184,25 +208,27 @@
 
             except sqlite3.Error as e:
                 return (0, e)
 
     def show_tables(self) -> tuple:
         try:
             with self.conn:
-                self.c.execute("SELECT name FROM sqlite_master WHERE type= 'table' ")
+                self.c.execute(
+                    "SELECT name FROM sqlite_master WHERE type= 'table' ")
                 for row in self.c.fetchall():
                     yield row
 
         except sqlite3.Error as e:
             return (0, e)
 
     def dropall(self):
         try:
             with self.conn:
-                self.c.execute("SELECT name FROM sqlite_master WHERE type= 'table' ")
+                self.c.execute(
+                    "SELECT name FROM sqlite_master WHERE type= 'table' ")
                 for table in self.c.fetchall():
                     self.c.execute(f'DROP TABLE {table[0]}')
                 return 1
 
         except sqlite3.Error as e:
             return (0, e)
 
@@ -225,21 +251,23 @@
             except sqlite3.Error as e:
                 return (0, e)
 
     def drop_content(self, ID, optional_table_name=None):
         if optional_table_name is None:
             try:
                 with self.conn:
-                    self.c.execute(f'DELETE FROM {self.tablename} WHERE ID = {ID}')
+                    self.c.execute(
+                        f'DELETE FROM {self.tablename} WHERE ID = {ID}')
                 return 11
 
             except sqlite3.Error as e:
                 return (0.0, e)
 
         else:
             try:
                 with self.conn:
-                    self.c.execute(f'DELETE FROM {optional_table_name} WHERE ID = {ID}')
+                    self.c.execute(
+                        f'DELETE FROM {optional_table_name} WHERE ID = {ID}')
                 return 1
 
             except sqlite3.Error as e:
                 return (0, e)
```

### Comparing `AshCrypt-1.3.4/AshCrypt/FileCrypt.py` & `AshCrypt-1.3.5/AshCrypt/FileCrypt.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 from AshCrypt import Ash
 import os
 
+
 class KeyError(Exception):
     def __init__(self):
         self.display = 'Key must be 512 Bit long !'
         super().__init__(self.display)
 
+
 class CryptFile():
-    def __init__(self,filename,key):
+    def __init__(self, filename, key):
         self.filename = filename
         self.not_512_bit_key = 0
         if self.keyverify(key) == 1:
             self.key = key
         else:
             self.not_512_bit_key = 1  # Raise KeyError()
 
@@ -24,20 +26,20 @@
         try:
             if isinstance(key, str):
                 a = bytes.fromhex(key.strip())
                 if len(a) == 64:
                     return 1
                 else:
                     return 0
-        except:
+        except BaseException:
             return 2
 
     def encrypt(self) -> int:
         if os.path.isdir(self.filename):
-            return  7
+            return 7
         if self.not_512_bit_key == 1:
             return 5
         try:
             go_ahead_rename_crypt = 0
             if not os.path.exists(self.filename):
                 return 3
             else:
@@ -45,33 +47,34 @@
                     return 6
                 else:
                     with open(self.filename, 'rb') as f:
                         filecontent = f.read()
                     with open(self.filename, 'wb') as f:
                         if filecontent:
                             try:
-                                ins = Ash.Enc(message=filecontent, mainkey=self.key)
+                                ins = Ash.Enc(
+                                    message=filecontent, mainkey=self.key)
                                 new_content = ins.encToBytes()
                                 f.write(new_content)
                                 go_ahead_rename_crypt = 1
-                            except:
+                            except BaseException:
                                 f.write(filecontent)
                                 return 0
                         else:
                             f.write(filecontent)
                             return 2
                     if go_ahead_rename_crypt == 1:
                         os.rename(self.filename, self.filename + '.crypt')
                         return 1
         except Exception:
             return 4
 
     def decrypt(self) -> int:
         if os.path.isdir(self.filename):
-            return  7
+            return 7
         if self.not_512_bit_key == 1:
             return 5
         try:
             go_ahead_remove_crypt = 0
             if not os.path.exists(self.filename):
                 return 3
             else:
@@ -79,29 +82,31 @@
                     return 6
                 else:
                     with open(self.filename, 'rb') as f:
                         enc_content = f.read()
                     with open(self.filename, 'wb') as f:
                         if enc_content:
                             try:
-                                ins = Ash.Dec(message=enc_content, mainkey=self.key)
+                                ins = Ash.Dec(
+                                    message=enc_content, mainkey=self.key)
                                 a = ins.decToBytes()
                                 f.write(a)
                                 go_ahead_remove_crypt = 1
                             except Exception:
                                 f.write(enc_content)
                                 return 0
                         else:
                             f.write(enc_content)
                             return 2
                     if go_ahead_remove_crypt == 1:
-                        os.rename(self.filename, os.path.splitext(self.filename)[0])
+                        os.rename(
+                            self.filename, os.path.splitext(
+                                self.filename)[0])
                         return 1
         except Exception:
             return 4
 
     def __str__(self):
         return f'Encrypting/Decrypting File {self.filename} With {self.key} Key '
+
     def __repr__(self):
         return f'{self.__class__.__name__}({self.filename},{self.key})'
-
-
```

### Comparing `AshCrypt-1.3.4/AshCrypt/README.md` & `AshCrypt-1.3.5/AshCrypt/README.md`

 * *Files identical despite different names*

### Comparing `AshCrypt-1.3.4/AshCrypt/TextCrypt.py` & `AshCrypt-1.3.5/AshCrypt/TextCrypt.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,62 +3,63 @@
 
 
 class KeyError(Exception):
     def __init__(self):
         self.display = 'Key must be 512 Bit long !'
         super().__init__(self.display)
 
+
 class Crypt():
-    def __init__(self,text: Union[str,bytes],key : str):
+    def __init__(self, text: Union[str, bytes], key: str):
         self.text = text
         if self.keyverify(key) == 1:
             self.key = key
         else:
             raise KeyError()
 
     @staticmethod
     def genkey() -> str:
         return Ash.Enc.genMainkey()
 
     @staticmethod
     def keyverify(key: str) -> int:
         if isinstance(key, str):
-            try :
+            try:
                 a = bytes.fromhex(key.strip())
-                if len(a) == 64 :
+                if len(a) == 64:
                     return 1
-            except Exception :
+            except Exception:
                 return 0
 
         else:
             return 2
 
-    def encrypt(self) -> tuple :
-            if self.text:
-                try:
-                    ins = Ash.Enc(self.text,self.key)
-                    new_content = ins.encToStr()
-                    return 1,new_content
-                except:
-                    output = 'E'
-                    return 0,output
-            else:
-                return 0.0,0.0
+    def encrypt(self) -> tuple:
+        if self.text:
+            try:
+                ins = Ash.Enc(self.text, self.key)
+                new_content = ins.encToStr()
+                return 1, new_content
+            except BaseException:
+                output = 'E'
+                return 0, output
+        else:
+            return 0.0, 0.0
 
-    def decrypt(self) -> tuple :
+    def decrypt(self) -> tuple:
         if self.text:
-                try:
-                    dec_instance = Ash.Dec(message=self.text,mainkey=self.key)
-                    a = dec_instance.decToStr()
-                    output = (a)
-                    return 1,output
-                except Exception:
-                    output = (self.text)
-                    return 0,output
+            try:
+                dec_instance = Ash.Dec(message=self.text, mainkey=self.key)
+                a = dec_instance.decToStr()
+                output = (a)
+                return 1, output
+            except Exception:
+                output = (self.text)
+                return 0, output
         else:
-            return 0.0,0.0
+            return 0.0, 0.0
 
     def __str__(self):
         return f'Encrypting/Decrypting Text {(self.text)[:8]}.. With {self.key} Key '
+
     def __repr__(self):
         return f'{self.__class__.__name__}({(self.text)[:8]},{self.key})'
-
```

### Comparing `AshCrypt-1.3.4/AshCrypt/__pycache__/Ash.cpython-39.pyc` & `AshCrypt-1.3.5/AshCrypt/__pycache__/Ash.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Sun Jul  2 19:28:38 2023 UTC, .py size: 4985 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 e6cf a164 7913 0000  a..........dy...
+00000000: 610d 0d0a 0000 0000 0833 ab64 5914 0000  a........3.dY...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 b000 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 6d03 5a03  d.l.m.Z.m.Z.m.Z.
 00000040: 0100 6400 6402 6c04 6d05 5a05 0100 6400  ..d.d.l.m.Z...d.
 00000050: 6403 6c06 6d07 5a07 0100 6400 6404 6c04  d.l.m.Z...d.d.l.
 00000060: 6d08 5a08 6d09 5a09 0100 6400 6405 6c0a  m.Z.m.Z...d.d.l.
 00000070: 6d0b 5a0b 0100 6400 6406 6c09 5a0c 6400  m.Z...d.d.l.Z.d.
@@ -28,30 +28,30 @@
 000001b0: 0000 0000 0000 0002 0000 0003 0000 0003  ................
 000001c0: 0000 0073 2000 0000 6401 7c01 9b00 6402  ...s ...d.|...d.
 000001d0: 9d03 7c00 5f00 7401 8300 a002 7c00 6a00  ..|._.t.....|.j.
 000001e0: a101 0100 6400 5300 2903 4e7a 3549 7465  ....d.S.).Nz5Ite
 000001f0: 7261 7469 6f6e 7320 6d75 7374 2062 6520  rations must be 
 00000200: 6265 7477 6565 6e20 3530 2061 6e64 2031  between 50 and 1
 00000210: 3030 3030 302e 2052 4543 4549 5645 4420  00000. RECEIVED 
-00000220: 3a20 fa01 20a9 035a 0764 6973 706c 6179  : .. ..Z.display
+00000220: 3a20 fa01 20a9 03da 0764 6973 706c 6179  : .. ....display
 00000230: da05 7375 7065 72da 085f 5f69 6e69 745f  ..super..__init_
 00000240: 5f29 02da 0473 656c 6672 0b00 0000 a901  _)...selfr......
 00000250: da09 5f5f 636c 6173 735f 5fa9 00fa 2a43  ..__class__...*C
 00000260: 3a5c 576f 726b 5c47 6974 4875 6257 6f72  :\Work\GitHubWor
 00000270: 6b5c 4145 532d 3235 365c 4173 6843 7279  k\AES-256\AshCry
-00000280: 7074 5c41 7368 2e70 7972 1000 0000 0d00  pt\Ash.pyr......
+00000280: 7074 5c41 7368 2e70 7972 1100 0000 0e00  pt\Ash.pyr......
 00000290: 0000 7304 0000 0000 010e 017a 2349 7465  ..s........z#Ite
 000002a0: 7261 7469 6f6e 734f 7574 6f66 6152 616e  rationsOutofaRan
 000002b0: 6765 4572 726f 722e 5f5f 696e 6974 5f5f  geError.__init__
 000002c0: 2906 da08 5f5f 6e61 6d65 5f5f da0a 5f5f  )...__name__..__
 000002d0: 6d6f 6475 6c65 5f5f da0c 5f5f 7175 616c  module__..__qual
-000002e0: 6e61 6d65 5f5f da03 616e 7972 1000 0000  name__..anyr....
+000002e0: 6e61 6d65 5f5f da03 616e 7972 1100 0000  name__..anyr....
 000002f0: da0d 5f5f 636c 6173 7363 656c 6c5f 5f72  ..__classcell__r
-00000300: 1400 0000 7214 0000 0072 1200 0000 7215  ....r....r....r.
-00000310: 0000 0072 0a00 0000 0c00 0000 7302 0000  ...r........s...
+00000300: 1500 0000 7215 0000 0072 1300 0000 7216  ....r....r....r.
+00000310: 0000 0072 0a00 0000 0d00 0000 7302 0000  ...r........s...
 00000320: 0008 0172 0a00 0000 6300 0000 0000 0000  ...r....c.......
 00000330: 0000 0000 0000 0000 0006 0000 0040 0000  .............@..
 00000340: 0073 bc00 0000 6500 5a01 6400 5a02 6503  .s....e.Z.d.Z.e.
 00000350: 6504 6505 6602 1900 6504 6401 6402 9c03  e.e.f...e.d.d...
 00000360: 6403 6404 8404 5a06 6507 6504 6505 6508  d.d...Z.e.e.e.e.
 00000370: 6505 6405 9c04 6406 6407 8404 8301 5a09  e.d...d.d.....Z.
 00000380: 6507 6504 6408 9c01 6409 640a 8404 8301  e.e.d...d.d.....
@@ -75,322 +75,325 @@
 000004a0: 6a7c 006a 0b64 036b 0472 7474 0c7c 006a  j|.j.d.k.rtt.|.j
 000004b0: 0b83 0182 017c 00a0 0d7c 006a 057c 006a  .....|...|.j.|.j
 000004c0: 097c 006a 0ba1 037c 005f 0e7c 00a0 0d7c  .|.j...|._.|...|
 000004d0: 006a 057c 006a 0a7c 006a 0ba1 037c 005f  .j.|.j.|.j...|._
 000004e0: 0f64 0053 0029 044e e910 0000 00e9 3200  .d.S.).N......2.
 000004f0: 0000 e9a0 8601 0029 10da 0a69 7369 6e73  .......)...isins
 00000500: 7461 6e63 65da 0373 7472 da06 656e 636f  tance..str..enco
-00000510: 6465 721d 0000 00da 0562 7974 6573 721e  der......bytesr.
+00000510: 6465 721e 0000 00da 0562 7974 6573 721f  der......bytesr.
 00000520: 0000 00da 026f 73da 0775 7261 6e64 6f6d  .....os..urandom
 00000530: da02 6976 da04 7361 6c74 da06 7065 7070  ..iv..salt..pepp
 00000540: 6572 da0a 6974 6572 6174 696f 6e73 720a  er..iterationsr.
 00000550: 0000 00da 0664 6572 6b65 79da 0665 6e63  .....derkey..enc
 00000560: 4b65 79da 0868 6d61 635f 6b65 7929 0372  Key..hmac_key).r
-00000570: 1100 0000 721d 0000 0072 1e00 0000 7214  ....r....r....r.
-00000580: 0000 0072 1400 0000 7215 0000 0072 1000  ...r....r....r..
-00000590: 0000 1200 0000 731a 0000 0000 010a 010c  ......s.........
+00000570: 1200 0000 721e 0000 0072 1f00 0000 7215  ....r....r....r.
+00000580: 0000 0072 1500 0000 7216 0000 0072 1100  ...r....r....r..
+00000590: 0000 1400 0000 731a 0000 0000 010a 010c  ......s.........
 000005a0: 010a 0106 0206 010c 010c 010c 0106 0114  ................
 000005b0: 010a 0116 017a 0c45 6e63 2e5f 5f69 6e69  .....z.Enc.__ini
-000005c0: 745f 5f29 0472 1e00 0000 da0b 7361 6c74  t__).r......salt
-000005d0: 5f70 6570 7065 7272 2b00 0000 720c 0000  _pepperr+...r...
+000005c0: 745f 5f29 0472 1f00 0000 da0b 7361 6c74  t__).r......salt
+000005d0: 5f70 6570 7065 7272 2c00 0000 720c 0000  _pepperr,...r...
 000005e0: 0063 0300 0000 0000 0000 0000 0000 0300  .c..............
 000005f0: 0000 0600 0000 4300 0000 7318 0000 0074  ......C...s....t
 00000600: 006a 017c 00a0 0264 01a1 017c 0164 027c  .j.|...d...|.d.|
 00000610: 0264 038d 0453 0029 044e fa05 5554 462d  .d...S.).N..UTF-
 00000620: 38e9 2000 0000 2904 5a08 7061 7373 776f  8. ...).Z.passwo
-00000630: 7264 7229 0000 005a 1164 6573 6972 6564  rdr)...Z.desired
+00000630: 7264 722a 0000 005a 1164 6573 6972 6564  rdr*...Z.desired
 00000640: 5f6b 6579 5f62 7974 6573 da06 726f 756e  _key_bytes..roun
 00000650: 6473 2903 da06 6263 7279 7074 5a03 6b64  ds)...bcryptZ.kd
-00000660: 6672 2400 0000 2903 721e 0000 0072 2f00  fr$...).r....r/.
-00000670: 0000 722b 0000 0072 1400 0000 7214 0000  ..r+...r....r...
-00000680: 0072 1500 0000 722c 0000 0022 0000 0073  .r....r,..."...s
+00000660: 6672 2500 0000 2903 721f 0000 0072 3000  fr%...).r....r0.
+00000670: 0000 722c 0000 0072 1500 0000 7215 0000  ..r,...r....r...
+00000680: 0072 1600 0000 722d 0000 0024 0000 0073  .r....r-...$...s
 00000690: 0c00 0000 0002 0401 0801 0201 0201 02fc  ................
 000006a0: 7a0a 456e 632e 6465 726b 6579 a901 720c  z.Enc.derkey..r.
 000006b0: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
 000006c0: 0000 0000 0300 0000 4300 0000 730e 0000  ........C...s...
 000006d0: 0074 00a0 0164 01a1 01a0 02a1 0053 0029  .t...d.......S.)
-000006e0: 024e e940 0000 0029 0372 2600 0000 7227  .N.@...).r&...r'
-000006f0: 0000 00da 0368 6578 7214 0000 0072 1400  .....hexr....r..
-00000700: 0000 7214 0000 0072 1500 0000 da0a 6765  ..r....r......ge
-00000710: 6e4d 6169 6e6b 6579 2a00 0000 7302 0000  nMainkey*...s...
+000006e0: 024e e940 0000 0029 0372 2700 0000 7228  .N.@...).r'...r(
+000006f0: 0000 00da 0368 6578 7215 0000 0072 1500  .....hexr....r..
+00000700: 0000 7215 0000 0072 1600 0000 da0a 6765  ..r....r......ge
+00000710: 6e4d 6169 6e6b 6579 2c00 0000 7302 0000  nMainkey,...s...
 00000720: 0000 027a 0e45 6e63 2e67 656e 4d61 696e  ...z.Enc.genMain
 00000730: 6b65 7963 0100 0000 0000 0000 0000 0000  keyc............
 00000740: 0100 0000 0300 0000 4300 0000 730c 0000  ........C...s...
 00000750: 0074 00a0 017c 006a 02a1 0153 00a9 014e  .t...|.j...S...N
-00000760: 2903 7204 0000 00da 0343 4243 7228 0000  ).r......CBCr(..
-00000770: 00a9 0172 1100 0000 7214 0000 0072 1400  ...r....r....r..
-00000780: 0000 7215 0000 00da 046d 6f64 652e 0000  ..r......mode...
+00000760: 2903 7204 0000 00da 0343 4243 7229 0000  ).r......CBCr)..
+00000770: 00a9 0172 1200 0000 7215 0000 0072 1500  ...r....r....r..
+00000780: 0000 7216 0000 00da 046d 6f64 6530 0000  ..r......mode0..
 00000790: 0073 0200 0000 0001 7a08 456e 632e 6d6f  .s......z.Enc.mo
 000007a0: 6465 6301 0000 0000 0000 0000 0000 0001  dec.............
 000007b0: 0000 0005 0000 0043 0000 0073 1e00 0000  .......C...s....
 000007c0: 7400 7401 6a02 7c00 6a03 6401 8d01 7c00  t.t.j.|.j.d...|.
 000007d0: a004 a100 7405 8300 6402 8d03 5300 a903  ....t...d...S...
-000007e0: 4e29 01da 036b 6579 2902 723b 0000 005a  N)...key).r;...Z
+000007e0: 4e29 01da 036b 6579 2902 723c 0000 005a  N)...key).r<...Z
 000007f0: 0762 6163 6b65 6e64 2906 7202 0000 0072  .backend).r....r
-00000800: 0300 0000 da03 4145 5372 2d00 0000 723b  ......AESr-...r;
-00000810: 0000 0072 0600 0000 723a 0000 0072 1400  ...r....r:...r..
-00000820: 0000 7214 0000 0072 1500 0000 da06 6369  ..r....r......ci
-00000830: 7068 6572 3100 0000 7302 0000 0000 017a  pher1...s......z
-00000840: 0a45 6e63 2e63 6970 6865 7263 0100 0000  .Enc.cipherc....
-00000850: 0000 0000 0000 0000 0100 0000 0200 0000  ................
-00000860: 4300 0000 730c 0000 007c 00a0 00a1 00a0  C...s....|......
-00000870: 01a1 0053 0072 3800 0000 2902 723f 0000  ...S.r8...).r?..
-00000880: 005a 0965 6e63 7279 7074 6f72 723a 0000  .Z.encryptorr:..
-00000890: 0072 1400 0000 7214 0000 0072 1500 0000  .r....r....r....
-000008a0: da10 6369 7068 6572 5f65 6e63 7279 7074  ..cipher_encrypt
-000008b0: 6f72 3400 0000 7302 0000 0000 017a 1445  or4...s......z.E
-000008c0: 6e63 2e63 6970 6865 725f 656e 6372 7970  nc.cipher_encryp
-000008d0: 746f 7263 0100 0000 0000 0000 0000 0000  torc............
-000008e0: 0200 0000 0300 0000 4300 0000 7322 0000  ........C...s"..
-000008f0: 0074 00a0 0164 01a1 01a0 02a1 007d 017c  .t...d.......}.|
-00000900: 01a0 037c 006a 04a1 017c 01a0 05a1 0017  ...|.j...|......
-00000910: 0053 00a9 024e e980 0000 0029 0672 0500  .S...N.....).r..
-00000920: 0000 da05 504b 4353 37da 0670 6164 6465  ....PKCS7..padde
-00000930: 72da 0675 7064 6174 6572 1d00 0000 da08  r..updater......
-00000940: 6669 6e61 6c69 7a65 2902 7211 0000 0072  finalize).r....r
-00000950: 4400 0000 7214 0000 0072 1400 0000 7215  D...r....r....r.
-00000960: 0000 00da 0e70 6164 6465 645f 6d65 7373  .....padded_mess
-00000970: 6167 6537 0000 0073 0400 0000 0001 0e01  age7...s........
-00000980: 7a12 456e 632e 7061 6464 6564 5f6d 6573  z.Enc.padded_mes
-00000990: 7361 6765 6301 0000 0000 0000 0000 0000  sagec...........
-000009a0: 0001 0000 0004 0000 0043 0000 0073 1e00  .........C...s..
-000009b0: 0000 7c00 a000 a100 a001 7c00 a002 a100  ..|.......|.....
-000009c0: a101 7c00 a000 a100 a003 a100 1700 5300  ..|...........S.
-000009d0: 7238 0000 0029 0472 4000 0000 7245 0000  r8...).r@...rE..
-000009e0: 0072 4700 0000 7246 0000 0072 3a00 0000  .rG...rF...r:...
-000009f0: 7214 0000 0072 1400 0000 7215 0000 00da  r....r....r.....
-00000a00: 0a63 6970 6865 7274 6578 743b 0000 0073  .ciphertext;...s
-00000a10: 0200 0000 0001 7a0e 456e 632e 6369 7068  ......z.Enc.ciph
-00000a20: 6572 7465 7874 6301 0000 0000 0000 0000  ertextc.........
-00000a30: 0000 0002 0000 0005 0000 0043 0000 0073  ...........C...s
-00000a40: 2c00 0000 7c00 6a00 7d01 7401 a002 7c01  ,...|.j.}.t...|.
-00000a50: 7403 a004 a100 a102 7d01 7c01 a005 7c00  t.......}.|...|.
-00000a60: a006 a100 a101 0100 7c01 a007 a100 5300  ........|.....S.
-00000a70: 7238 0000 0029 0872 2e00 0000 7208 0000  r8...).r....r...
-00000a80: 00da 0448 4d41 4372 0700 0000 da06 5348  ...HMACr......SH
-00000a90: 4135 3132 7245 0000 0072 4800 0000 7246  A512rE...rH...rF
-00000aa0: 0000 00a9 0272 1100 0000 da01 6872 1400  .....r......hr..
-00000ab0: 0000 7214 0000 0072 1500 0000 7249 0000  ..r....r....rI..
-00000ac0: 003e 0000 0073 0800 0000 0001 0601 1001  .>...s..........
-00000ad0: 0e01 7a08 456e 632e 484d 4143 6301 0000  ..z.Enc.HMACc...
-00000ae0: 0000 0000 0000 0000 0002 0000 0004 0000  ................
-00000af0: 0043 0000 0073 1200 0000 7400 a001 6401  .C...s....t...d.
-00000b00: 7c00 6a02 a102 7d01 7c01 5300 2902 4efa  |.j...}.|.S.).N.
-00000b10: 0221 4929 03da 0673 7472 7563 74da 0470  .!I)...struct..p
-00000b20: 6163 6b72 2b00 0000 2902 7211 0000 005a  ackr+...).r....Z
-00000b30: 0b69 7465 7273 5f62 7974 6573 7214 0000  .iters_bytesr...
-00000b40: 0072 1400 0000 7215 0000 00da 0f73 6574  .r....r......set
-00000b50: 7570 4974 6572 6174 696f 6e73 4400 0000  upIterationsD...
-00000b60: 7304 0000 0000 010e 017a 1345 6e63 2e73  s........z.Enc.s
-00000b70: 6574 7570 4974 6572 6174 696f 6e73 6301  etupIterationsc.
-00000b80: 0000 0000 0000 0000 0000 0001 0000 0003  ................
-00000b90: 0000 0043 0000 0073 2a00 0000 7c00 a000  ...C...s*...|...
-00000ba0: a100 7c00 6a01 1700 7c00 6a02 1700 7c00  ..|.j...|.j...|.
-00000bb0: 6a03 1700 7c00 a004 a100 1700 7c00 a005  j...|.......|...
-00000bc0: a100 1700 5300 7238 0000 0029 0672 4900  ....S.r8...).rI.
-00000bd0: 0000 7228 0000 0072 2900 0000 722a 0000  ..r(...r)...r*..
-00000be0: 0072 5000 0000 7248 0000 0072 3a00 0000  .rP...rH...r:...
-00000bf0: 7214 0000 0072 1400 0000 7215 0000 00da  r....r....r.....
-00000c00: 0a65 6e63 546f 4279 7465 7348 0000 0073  .encToBytesH...s
-00000c10: 0200 0000 0001 7a0e 456e 632e 656e 6354  ......z.Enc.encT
-00000c20: 6f42 7974 6573 6301 0000 0000 0000 0000  oBytesc.........
-00000c30: 0000 0001 0000 0004 0000 0043 0000 0073  ...........C...s
-00000c40: 1400 0000 7400 a001 7c00 a002 a100 a101  ....t...|.......
-00000c50: a003 6401 a101 5300 a902 4e72 3000 0000  ..d...S...Nr0...
-00000c60: 2904 da06 6261 7365 3634 5a11 7572 6c73  )...base64Z.urls
-00000c70: 6166 655f 6236 3465 6e63 6f64 6572 5100  afe_b64encoderQ.
-00000c80: 0000 da06 6465 636f 6465 723a 0000 0072  ....decoder:...r
-00000c90: 1400 0000 7214 0000 0072 1500 0000 da08  ....r....r......
-00000ca0: 656e 6354 6f53 7472 4b00 0000 7302 0000  encToStrK...s...
-00000cb0: 0000 017a 0c45 6e63 2e65 6e63 546f 5374  ...z.Enc.encToSt
-00000cc0: 7229 1472 1600 0000 7217 0000 0072 1800  r).r....r....r..
-00000cd0: 0000 7209 0000 0072 2300 0000 7225 0000  ..r....r#...r%..
-00000ce0: 0072 1000 0000 da0c 7374 6174 6963 6d65  .r......staticme
-00000cf0: 7468 6f64 da03 696e 7472 2c00 0000 7237  thod..intr,...r7
-00000d00: 0000 0072 3b00 0000 723f 0000 0072 4000  ...r;...r?...r@.
-00000d10: 0000 7247 0000 0072 4800 0000 7249 0000  ..rG...rH...rI..
-00000d20: 0072 5000 0000 7251 0000 0072 5500 0000  .rP...rQ...rU...
-00000d30: 7214 0000 0072 1400 0000 7214 0000 0072  r....r....r....r
-00000d40: 1500 0000 721b 0000 0011 0000 0073 1c00  ....r........s..
-00000d50: 0000 0801 1a10 0201 1607 0201 1003 0803  ................
-00000d60: 0803 0803 0e04 0e03 0e06 0e04 0e03 721b  ..............r.
-00000d70: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
-00000d80: 0000 0000 0400 0000 0000 0000 7322 0000  ............s"..
-00000d90: 0065 005a 0164 005a 0264 0164 029c 0187  .e.Z.d.Z.d.d....
-00000da0: 0066 0164 0364 0484 0c5a 0387 0004 005a  .f.d.d...Z.....Z
-00000db0: 0453 0029 05da 154d 6573 7361 6765 5461  .S.)...MessageTa
-00000dc0: 6d70 6572 696e 6745 7272 6f72 4e72 3400  mperingErrorNr4.
-00000dd0: 0000 6301 0000 0000 0000 0000 0000 0001  ..c.............
-00000de0: 0000 0003 0000 0003 0000 0073 1800 0000  ...........s....
-00000df0: 6401 7c00 5f00 7401 8300 a002 7c00 6a00  d.|._.t.....|.j.
-00000e00: a101 0100 6400 5300 2902 4e7a 4c48 4d41  ....d.S.).NzLHMA
-00000e10: 4320 6d69 736d 6174 6368 2021 204d 6573  C mismatch ! Mes
-00000e20: 7361 6765 2068 6173 2062 6565 6e20 5441  sage has been TA
-00000e30: 4d50 4552 4544 2077 6974 6820 2c0a 206f  MPERED with ,. o
-00000e40: 7220 506f 7373 6962 6c65 206b 6579 2064  r Possible key d
-00000e50: 6966 6665 7265 6e63 6572 0e00 0000 723a  ifferencer....r:
-00000e60: 0000 0072 1200 0000 7214 0000 0072 1500  ...r....r....r..
-00000e70: 0000 7210 0000 0050 0000 0073 0400 0000  ..r....P...s....
-00000e80: 0001 0601 7a1e 4d65 7373 6167 6554 616d  ....z.MessageTam
-00000e90: 7065 7269 6e67 4572 726f 722e 5f5f 696e  peringError.__in
-00000ea0: 6974 5f5f 2905 7216 0000 0072 1700 0000  it__).r....r....
-00000eb0: 7218 0000 0072 1000 0000 721a 0000 0072  r....r....r....r
-00000ec0: 1400 0000 7214 0000 0072 1200 0000 7215  ....r....r....r.
-00000ed0: 0000 0072 5800 0000 4f00 0000 7302 0000  ...rX...O...s...
-00000ee0: 0008 0172 5800 0000 6300 0000 0000 0000  ...rX...c.......
-00000ef0: 0000 0000 0000 0000 0004 0000 0040 0000  .............@..
-00000f00: 0073 9200 0000 6500 5a01 6400 5a02 6503  .s....e.Z.d.Z.e.
-00000f10: 6504 6505 6602 1900 6504 6401 6402 9c03  e.e.f...e.d.d...
-00000f20: 6403 6404 8404 5a06 6505 6405 9c01 6406  d.d...Z.e.d...d.
-00000f30: 6407 8404 5a07 6508 6405 9c01 6408 6409  d...Z.e.d...d.d.
-00000f40: 8404 5a09 640a 640b 8400 5a0a 640c 640d  ..Z.d.d...Z.d.d.
-00000f50: 8400 5a0b 640e 640f 8400 5a0c 6505 6405  ..Z.d.d...Z.e.d.
-00000f60: 9c01 6410 6411 8404 5a0d 6505 6405 9c01  ..d.d...Z.e.d...
-00000f70: 6412 6413 8404 5a0e 6505 6405 9c01 6414  d.d...Z.e.d...d.
-00000f80: 6415 8404 5a0f 6504 6405 9c01 6416 6417  d...Z.e.d...d.d.
-00000f90: 8404 5a10 6401 5300 2918 da03 4465 634e  ..Z.d.S.)...DecN
-00000fa0: 721c 0000 0063 0300 0000 0000 0000 0000  r....c..........
-00000fb0: 0000 0400 0000 0600 0000 4300 0000 7306  ..........C...s.
-00000fc0: 0100 0074 007c 0174 0183 0272 227c 01a0  ...t.|.t...r"|..
-00000fd0: 0264 01a1 017d 0374 03a0 047c 03a1 017c  .d...}.t...|...|
-00000fe0: 005f 056e 1074 007c 0174 0683 0272 327c  ._.n.t.|.t...r2|
-00000ff0: 017c 005f 057c 027c 005f 077c 006a 0564  .|._.|.|._.|.j.d
-00001000: 0064 0285 0219 007c 005f 087c 006a 0564  .d.....|._.|.j.d
-00001010: 0264 0385 0219 007c 005f 097c 006a 0564  .d.....|._.|.j.d
-00001020: 0364 0485 0219 007c 005f 0a7c 006a 0564  .d.....|._.|.j.d
-00001030: 0464 0585 0219 007c 005f 0b74 0ca0 0d64  .d.....|._.t...d
-00001040: 067c 006a 0564 0564 0785 0219 00a1 0264  .|.j.d.d.......d
-00001050: 0819 007c 005f 0e7c 006a 0e64 096b 0073  ...|._.|.j.d.k.s
-00001060: a87c 006a 0e64 0a6b 0472 b274 0f7c 006a  .|.j.d.k.r.t.|.j
-00001070: 0e83 0182 017c 006a 0564 0764 0085 0219  .....|.j.d.d....
-00001080: 007c 005f 1074 11a0 127c 006a 077c 006a  .|._.t...|.j.|.j
-00001090: 0a7c 006a 0ea1 037c 005f 1374 11a0 127c  .|.j...|._.t...|
-000010a0: 006a 077c 006a 0b7c 006a 0ea1 037c 005f  .j.|.j.|.j...|._
-000010b0: 147c 00a0 15a1 0064 0b75 0090 0172 0274  .|.....d.u...r.t
-000010c0: 1683 0082 0164 0053 0029 0c4e 7230 0000  .....d.S.).Nr0..
-000010d0: 0072 3500 0000 e950 0000 00e9 6000 0000  .r5....P....`...
-000010e0: e970 0000 0072 4d00 0000 e974 0000 0072  .p...rM....t...r
-000010f0: 0100 0000 7220 0000 0072 2100 0000 4629  ....r ...r!...F)
-00001100: 1772 2200 0000 7223 0000 0072 2400 0000  .r"...r#...r$...
-00001110: 7253 0000 005a 1175 726c 7361 6665 5f62  rS...Z.urlsafe_b
-00001120: 3634 6465 636f 6465 721d 0000 0072 2500  64decoder....r%.
-00001130: 0000 723d 0000 00da 0872 6563 5f68 6d61  ..r=.....rec_hma
-00001140: 63da 0672 6563 5f69 76da 0872 6563 5f73  c..rec_iv..rec_s
-00001150: 616c 74da 0a72 6563 5f70 6570 7065 7272  alt..rec_pepperr
-00001160: 4e00 0000 da06 756e 7061 636b da0e 7265  N.....unpack..re
-00001170: 635f 6974 6572 6174 696f 6e73 720a 0000  c_iterationsr...
-00001180: 00da 0e72 6563 5f63 6970 6865 7274 6578  ...rec_ciphertex
-00001190: 7472 1b00 0000 722c 0000 00da 0664 6563  tr....r,.....dec
-000011a0: 4b65 79da 0668 6d61 635f 6bda 0a76 6572  Key..hmac_k..ver
-000011b0: 6966 7948 4d41 4372 5800 0000 2904 7211  ifyHMACrX...).r.
-000011c0: 0000 0072 1d00 0000 721e 0000 00da 016d  ...r....r......m
-000011d0: 7214 0000 0072 1400 0000 7215 0000 0072  r....r....r....r
-000011e0: 1000 0000 5500 0000 7324 0000 0000 010a  ....U...s$......
-000011f0: 010a 010e 010a 0106 0106 0110 0110 0110  ................
-00001200: 0110 011c 0114 010a 0110 0116 0116 010e  ................
-00001210: 017a 0c44 6563 2e5f 5f69 6e69 745f 5f72  .z.Dec.__init__r
-00001220: 3400 0000 6301 0000 0000 0000 0000 0000  4...c...........
-00001230: 0002 0000 0005 0000 0043 0000 0073 2a00  .........C...s*.
-00001240: 0000 7c00 6a00 7d01 7401 a002 7c01 7403  ..|.j.}.t...|.t.
-00001250: a004 a100 a102 7d01 7c01 a005 7c00 6a06  ......}.|...|.j.
-00001260: a101 0100 7c01 a007 a100 5300 7238 0000  ....|.....S.r8..
-00001270: 0029 0872 6600 0000 7208 0000 0072 4900  .).rf...r....rI.
-00001280: 0000 7207 0000 0072 4a00 0000 7245 0000  ..r....rJ...rE..
-00001290: 0072 6400 0000 7246 0000 0072 4b00 0000  .rd...rF...rK...
-000012a0: 7214 0000 0072 1400 0000 7215 0000 00da  r....r....r.....
-000012b0: 0a61 6374 7561 6c48 4d41 4368 0000 0073  .actualHMACh...s
-000012c0: 0800 0000 0001 0601 1001 0c01 7a0e 4465  ............z.De
-000012d0: 632e 6163 7475 616c 484d 4143 6301 0000  c.actualHMACc...
-000012e0: 0000 0000 0000 0000 0001 0000 0004 0000  ................
-000012f0: 0043 0000 0073 1200 0000 7400 a001 7c00  .C...s....t...|.
-00001300: a002 a100 7c00 6a03 a102 5300 7238 0000  ....|.j...S.r8..
-00001310: 0029 04da 0368 6d63 5a0e 636f 6d70 6172  .)...hmcZ.compar
-00001320: 655f 6469 6765 7374 7269 0000 0072 5e00  e_digestri...r^.
-00001330: 0000 723a 0000 0072 1400 0000 7214 0000  ..r:...r....r...
-00001340: 0072 1500 0000 7267 0000 006e 0000 0073  .r....rg...n...s
-00001350: 0200 0000 0001 7a0e 4465 632e 7665 7269  ......z.Dec.veri
-00001360: 6679 484d 4143 6301 0000 0000 0000 0000  fyHMACc.........
-00001370: 0000 0001 0000 0003 0000 0043 0000 0073  ...........C...s
-00001380: 0c00 0000 7400 a001 7c00 6a02 a101 5300  ....t...|.j...S.
-00001390: 7238 0000 0029 0372 0400 0000 7239 0000  r8...).r....r9..
-000013a0: 0072 5f00 0000 723a 0000 0072 1400 0000  .r_...r:...r....
-000013b0: 7214 0000 0072 1500 0000 723b 0000 0071  r....r....r;...q
-000013c0: 0000 0073 0200 0000 0001 7a08 4465 632e  ...s......z.Dec.
-000013d0: 6d6f 6465 6301 0000 0000 0000 0000 0000  modec...........
-000013e0: 0001 0000 0005 0000 0043 0000 0073 1e00  .........C...s..
-000013f0: 0000 7400 7401 6a02 7c00 6a03 6401 8d01  ..t.t.j.|.j.d...
-00001400: 7c00 a004 a100 7405 8300 6402 8d03 5300  |.....t...d...S.
-00001410: 723c 0000 0029 0672 0200 0000 7203 0000  r<...).r....r...
-00001420: 0072 3e00 0000 7265 0000 0072 3b00 0000  .r>...re...r;...
-00001430: 7206 0000 0072 3a00 0000 7214 0000 0072  r....r:...r....r
-00001440: 1400 0000 7215 0000 0072 3f00 0000 7400  ....r....r?...t.
-00001450: 0000 7302 0000 0000 017a 0a44 6563 2e63  ..s......z.Dec.c
-00001460: 6970 6865 7263 0100 0000 0000 0000 0000  ipherc..........
-00001470: 0000 0100 0000 0200 0000 4300 0000 730c  ..........C...s.
-00001480: 0000 007c 00a0 00a1 00a0 01a1 0053 0072  ...|.........S.r
-00001490: 3800 0000 2902 723f 0000 005a 0964 6563  8...).r?...Z.dec
-000014a0: 7279 7074 6f72 723a 0000 0072 1400 0000  ryptorr:...r....
-000014b0: 7214 0000 0072 1500 0000 da10 6369 7068  r....r......ciph
-000014c0: 6572 5f64 6563 7279 7074 6f72 7700 0000  er_decryptorw...
-000014d0: 7302 0000 0000 017a 1444 6563 2e63 6970  s......z.Dec.cip
-000014e0: 6865 725f 6465 6372 7970 746f 7263 0100  her_decryptorc..
-000014f0: 0000 0000 0000 0000 0000 0100 0000 0300  ................
-00001500: 0000 4300 0000 731c 0000 007c 00a0 00a1  ..C...s....|....
-00001510: 00a0 017c 006a 02a1 017c 00a0 00a1 00a0  ...|.j...|......
-00001520: 03a1 0017 0053 0072 3800 0000 2904 726b  .....S.r8...).rk
-00001530: 0000 0072 4500 0000 7264 0000 0072 4600  ...rE...rd...rF.
-00001540: 0000 723a 0000 0072 1400 0000 7214 0000  ..r:...r....r...
-00001550: 0072 1500 0000 da11 7072 655f 756e 7061  .r......pre_unpa
-00001560: 6464 696e 675f 6465 637a 0000 0073 0200  dding_decz...s..
-00001570: 0000 0001 7a15 4465 632e 7072 655f 756e  ....z.Dec.pre_un
-00001580: 7061 6464 696e 675f 6465 6363 0100 0000  padding_decc....
-00001590: 0000 0000 0000 0000 0200 0000 0400 0000  ................
-000015a0: 4300 0000 7324 0000 0074 00a0 0164 01a1  C...s$...t...d..
-000015b0: 01a0 02a1 007d 017c 01a0 037c 00a0 04a1  .....}.|...|....
-000015c0: 00a1 017c 01a0 05a1 0017 0053 0072 4100  ...|.......S.rA.
-000015d0: 0000 2906 7205 0000 0072 4300 0000 da08  ..).r....rC.....
-000015e0: 756e 7061 6464 6572 7245 0000 0072 6c00  unpadderrE...rl.
-000015f0: 0000 7246 0000 0029 0272 1100 0000 726d  ..rF...).r....rm
-00001600: 0000 0072 1400 0000 7214 0000 0072 1500  ...r....r....r..
-00001610: 0000 da0a 756e 7061 6464 6564 5f6d 7d00  ....unpadded_m}.
-00001620: 0000 7304 0000 0000 010e 017a 0e44 6563  ..s........z.Dec
-00001630: 2e75 6e70 6164 6465 645f 6d63 0100 0000  .unpadded_mc....
-00001640: 0000 0000 0000 0000 0100 0000 0200 0000  ................
-00001650: 4300 0000 7308 0000 007c 00a0 00a1 0053  C...s....|.....S
-00001660: 0072 3800 0000 2901 726e 0000 0072 3a00  .r8...).rn...r:.
-00001670: 0000 7214 0000 0072 1400 0000 7215 0000  ..r....r....r...
-00001680: 00da 0a64 6563 546f 4279 7465 7381 0000  ...decToBytes...
-00001690: 0073 0200 0000 0001 7a0e 4465 632e 6465  .s......z.Dec.de
-000016a0: 6354 6f42 7974 6573 6301 0000 0000 0000  cToBytesc.......
-000016b0: 0000 0000 0001 0000 0003 0000 0043 0000  .............C..
-000016c0: 0073 0e00 0000 7c00 a000 a100 a001 6401  .s....|.......d.
-000016d0: a101 5300 7252 0000 0029 0272 6e00 0000  ..S.rR...).rn...
-000016e0: 7254 0000 0072 3a00 0000 7214 0000 0072  rT...r:...r....r
-000016f0: 1400 0000 7215 0000 00da 0864 6563 546f  ....r......decTo
-00001700: 5374 7284 0000 0073 0200 0000 0001 7a0c  Str....s......z.
-00001710: 4465 632e 6465 6354 6f53 7472 2911 7216  Dec.decToStr).r.
-00001720: 0000 0072 1700 0000 7218 0000 0072 0900  ...r....r....r..
-00001730: 0000 7223 0000 0072 2500 0000 7210 0000  ..r#...r%...r...
-00001740: 0072 6900 0000 da04 626f 6f6c 7267 0000  .ri.....boolrg..
-00001750: 0072 3b00 0000 723f 0000 0072 6b00 0000  .r;...r?...rk...
-00001760: 726c 0000 0072 6e00 0000 726f 0000 0072  rl...rn...ro...r
-00001770: 7000 0000 7214 0000 0072 1400 0000 7214  p...r....r....r.
-00001780: 0000 0072 1500 0000 7259 0000 0054 0000  ...r....rY...T..
-00001790: 0073 1400 0000 0801 1a13 0e06 0e03 0803  .s..............
-000017a0: 0803 0803 0e03 0e04 0e03 7259 0000 0029  ..........rY...)
-000017b0: 165a 2663 7279 7074 6f67 7261 7068 792e  .Z&cryptography.
-000017c0: 6861 7a6d 6174 2e70 7269 6d69 7469 7665  hazmat.primitive
-000017d0: 732e 6369 7068 6572 7372 0200 0000 7203  s.ciphersr....r.
-000017e0: 0000 0072 0400 0000 5a1e 6372 7970 746f  ...r....Z.crypto
-000017f0: 6772 6170 6879 2e68 617a 6d61 742e 7072  graphy.hazmat.pr
-00001800: 696d 6974 6976 6573 7205 0000 005a 1c63  imitivesr....Z.c
-00001810: 7279 7074 6f67 7261 7068 792e 6861 7a6d  ryptography.hazm
-00001820: 6174 2e62 6163 6b65 6e64 7372 0600 0000  at.backendsr....
-00001830: 7207 0000 0072 0800 0000 da06 7479 7069  r....r......typi
-00001840: 6e67 7209 0000 0072 6a00 0000 7233 0000  ngr....rj...r3..
-00001850: 0072 5300 0000 724e 0000 0072 2600 0000  .rS...rN...r&...
-00001860: da09 4578 6365 7074 696f 6e72 0a00 0000  ..Exceptionr....
-00001870: 721b 0000 0072 5800 0000 7259 0000 0072  r....rX...rY...r
-00001880: 1400 0000 7214 0000 0072 1400 0000 7215  ....r....r....r.
-00001890: 0000 00da 083c 6d6f 6475 6c65 3e01 0000  .....<module>...
-000018a0: 0073 1a00 0000 1401 0c01 0c01 1001 0c01  .s..............
-000018b0: 0801 0801 0801 0801 0802 1005 0e3e 1005  .............>..
+00000800: 0300 0000 da03 4145 5372 2e00 0000 723c  ......AESr....r<
+00000810: 0000 0072 0600 0000 723b 0000 0072 1500  ...r....r;...r..
+00000820: 0000 7215 0000 0072 1600 0000 da06 6369  ..r....r......ci
+00000830: 7068 6572 3300 0000 730e 0000 0000 0102  pher3...s.......
+00000840: 0104 0104 ff04 0206 0104 fc7a 0a45 6e63  ...........z.Enc
+00000850: 2e63 6970 6865 7263 0100 0000 0000 0000  .cipherc........
+00000860: 0000 0000 0100 0000 0200 0000 4300 0000  ............C...
+00000870: 730c 0000 007c 00a0 00a1 00a0 01a1 0053  s....|.........S
+00000880: 0072 3900 0000 2902 7240 0000 005a 0965  .r9...).r@...Z.e
+00000890: 6e63 7279 7074 6f72 723b 0000 0072 1500  ncryptorr;...r..
+000008a0: 0000 7215 0000 0072 1600 0000 da10 6369  ..r....r......ci
+000008b0: 7068 6572 5f65 6e63 7279 7074 6f72 3a00  pher_encryptor:.
+000008c0: 0000 7302 0000 0000 017a 1445 6e63 2e63  ..s......z.Enc.c
+000008d0: 6970 6865 725f 656e 6372 7970 746f 7263  ipher_encryptorc
+000008e0: 0100 0000 0000 0000 0000 0000 0200 0000  ................
+000008f0: 0300 0000 4300 0000 7322 0000 0074 00a0  ....C...s"...t..
+00000900: 0164 01a1 01a0 02a1 007d 017c 01a0 037c  .d.......}.|...|
+00000910: 006a 04a1 017c 01a0 05a1 0017 0053 00a9  .j...|.......S..
+00000920: 024e e980 0000 0029 0672 0500 0000 da05  .N.....).r......
+00000930: 504b 4353 37da 0670 6164 6465 72da 0675  PKCS7..padder..u
+00000940: 7064 6174 6572 1e00 0000 da08 6669 6e61  pdater......fina
+00000950: 6c69 7a65 2902 7212 0000 0072 4500 0000  lize).r....rE...
+00000960: 7215 0000 0072 1500 0000 7216 0000 00da  r....r....r.....
+00000970: 0e70 6164 6465 645f 6d65 7373 6167 653d  .padded_message=
+00000980: 0000 0073 0400 0000 0001 0e01 7a12 456e  ...s........z.En
+00000990: 632e 7061 6464 6564 5f6d 6573 7361 6765  c.padded_message
+000009a0: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
+000009b0: 0004 0000 0043 0000 0073 1e00 0000 7c00  .....C...s....|.
+000009c0: a000 a100 a001 7c00 a002 a100 a101 7c00  ......|.......|.
+000009d0: a000 a100 a003 a100 1700 5300 7239 0000  ..........S.r9..
+000009e0: 0029 0472 4100 0000 7246 0000 0072 4800  .).rA...rF...rH.
+000009f0: 0000 7247 0000 0072 3b00 0000 7215 0000  ..rG...r;...r...
+00000a00: 0072 1500 0000 7216 0000 00da 0a63 6970  .r....r......cip
+00000a10: 6865 7274 6578 7441 0000 0073 0600 0000  hertextA...s....
+00000a20: 0001 1001 0aff 7a0e 456e 632e 6369 7068  ......z.Enc.ciph
+00000a30: 6572 7465 7874 6301 0000 0000 0000 0000  ertextc.........
+00000a40: 0000 0002 0000 0005 0000 0043 0000 0073  ...........C...s
+00000a50: 2c00 0000 7c00 6a00 7d01 7401 a002 7c01  ,...|.j.}.t...|.
+00000a60: 7403 a004 a100 a102 7d01 7c01 a005 7c00  t.......}.|...|.
+00000a70: a006 a100 a101 0100 7c01 a007 a100 5300  ........|.....S.
+00000a80: 7239 0000 0029 0872 2f00 0000 7208 0000  r9...).r/...r...
+00000a90: 00da 0448 4d41 4372 0700 0000 da06 5348  ...HMACr......SH
+00000aa0: 4135 3132 7246 0000 0072 4900 0000 7247  A512rF...rI...rG
+00000ab0: 0000 00a9 0272 1200 0000 da01 6872 1500  .....r......hr..
+00000ac0: 0000 7215 0000 0072 1600 0000 724a 0000  ..r....r....rJ..
+00000ad0: 0045 0000 0073 0800 0000 0001 0601 1001  .E...s..........
+00000ae0: 0e01 7a08 456e 632e 484d 4143 6301 0000  ..z.Enc.HMACc...
+00000af0: 0000 0000 0000 0000 0002 0000 0004 0000  ................
+00000b00: 0043 0000 0073 1200 0000 7400 a001 6401  .C...s....t...d.
+00000b10: 7c00 6a02 a102 7d01 7c01 5300 2902 4efa  |.j...}.|.S.).N.
+00000b20: 0221 4929 03da 0673 7472 7563 745a 0470  .!I)...structZ.p
+00000b30: 6163 6b72 2c00 0000 2902 7212 0000 005a  ackr,...).r....Z
+00000b40: 0b69 7465 7273 5f62 7974 6573 7215 0000  .iters_bytesr...
+00000b50: 0072 1500 0000 7216 0000 00da 0f73 6574  .r....r......set
+00000b60: 7570 4974 6572 6174 696f 6e73 4b00 0000  upIterationsK...
+00000b70: 7304 0000 0000 010e 017a 1345 6e63 2e73  s........z.Enc.s
+00000b80: 6574 7570 4974 6572 6174 696f 6e73 6301  etupIterationsc.
+00000b90: 0000 0000 0000 0000 0000 0001 0000 0003  ................
+00000ba0: 0000 0043 0000 0073 2a00 0000 7c00 a000  ...C...s*...|...
+00000bb0: a100 7c00 6a01 1700 7c00 6a02 1700 7c00  ..|.j...|.j...|.
+00000bc0: 6a03 1700 7c00 a004 a100 1700 7c00 a005  j...|.......|...
+00000bd0: a100 1700 5300 7239 0000 0029 0672 4a00  ....S.r9...).rJ.
+00000be0: 0000 7229 0000 0072 2a00 0000 722b 0000  ..r)...r*...r+..
+00000bf0: 0072 5000 0000 7249 0000 0072 3b00 0000  .rP...rI...r;...
+00000c00: 7215 0000 0072 1500 0000 7216 0000 00da  r....r....r.....
+00000c10: 0a65 6e63 546f 4279 7465 734f 0000 0073  .encToBytesO...s
+00000c20: 0a00 0000 0001 1801 06ff 0201 06ff 7a0e  ..............z.
+00000c30: 456e 632e 656e 6354 6f42 7974 6573 6301  Enc.encToBytesc.
+00000c40: 0000 0000 0000 0000 0000 0001 0000 0004  ................
+00000c50: 0000 0043 0000 0073 1400 0000 7400 a001  ...C...s....t...
+00000c60: 7c00 a002 a100 a101 a003 6401 a101 5300  |.........d...S.
+00000c70: a902 4e72 3100 0000 2904 da06 6261 7365  ..Nr1...)...base
+00000c80: 3634 5a11 7572 6c73 6166 655f 6236 3465  64Z.urlsafe_b64e
+00000c90: 6e63 6f64 6572 5100 0000 da06 6465 636f  ncoderQ.....deco
+00000ca0: 6465 723b 0000 0072 1500 0000 7215 0000  der;...r....r...
+00000cb0: 0072 1600 0000 da08 656e 6354 6f53 7472  .r......encToStr
+00000cc0: 5300 0000 7302 0000 0000 017a 0c45 6e63  S...s......z.Enc
+00000cd0: 2e65 6e63 546f 5374 7229 1472 1700 0000  .encToStr).r....
+00000ce0: 7218 0000 0072 1900 0000 7209 0000 0072  r....r....r....r
+00000cf0: 2400 0000 7226 0000 0072 1100 0000 da0c  $...r&...r......
+00000d00: 7374 6174 6963 6d65 7468 6f64 da03 696e  staticmethod..in
+00000d10: 7472 2d00 0000 7238 0000 0072 3c00 0000  tr-...r8...r<...
+00000d20: 7240 0000 0072 4100 0000 7248 0000 0072  r@...rA...rH...r
+00000d30: 4900 0000 724a 0000 0072 5000 0000 7251  I...rJ...rP...rQ
+00000d40: 0000 0072 5500 0000 7215 0000 0072 1500  ...rU...r....r..
+00000d50: 0000 7215 0000 0072 1600 0000 721c 0000  ..r....r....r...
+00000d60: 0013 0000 0073 1c00 0000 0801 1a10 0201  .....s..........
+00000d70: 1607 0201 1003 0803 0807 0803 0e04 0e04  ................
+00000d80: 0e06 0e04 0e04 721c 0000 0063 0000 0000  ......r....c....
+00000d90: 0000 0000 0000 0000 0000 0000 0400 0000  ................
+00000da0: 0000 0000 7322 0000 0065 005a 0164 005a  ....s"...e.Z.d.Z
+00000db0: 0264 0164 029c 0187 0066 0164 0364 0484  .d.d.....f.d.d..
+00000dc0: 0c5a 0387 0004 005a 0453 0029 05da 154d  .Z.....Z.S.)...M
+00000dd0: 6573 7361 6765 5461 6d70 6572 696e 6745  essageTamperingE
+00000de0: 7272 6f72 4e72 3500 0000 6301 0000 0000  rrorNr5...c.....
+00000df0: 0000 0000 0000 0001 0000 0003 0000 0003  ................
+00000e00: 0000 0073 1800 0000 6401 7c00 5f00 7401  ...s....d.|._.t.
+00000e10: 8300 a002 7c00 6a00 a101 0100 6400 5300  ....|.j.....d.S.
+00000e20: 2902 4e7a 4c48 4d41 4320 6d69 736d 6174  ).NzLHMAC mismat
+00000e30: 6368 2021 204d 6573 7361 6765 2068 6173  ch ! Message has
+00000e40: 2062 6565 6e20 5441 4d50 4552 4544 2077   been TAMPERED w
+00000e50: 6974 6820 2c0a 206f 7220 506f 7373 6962  ith ,. or Possib
+00000e60: 6c65 206b 6579 2064 6966 6665 7265 6e63  le key differenc
+00000e70: 6572 0e00 0000 723b 0000 0072 1300 0000  er....r;...r....
+00000e80: 7215 0000 0072 1600 0000 7211 0000 0058  r....r....r....X
+00000e90: 0000 0073 0400 0000 0001 0601 7a1e 4d65  ...s........z.Me
+00000ea0: 7373 6167 6554 616d 7065 7269 6e67 4572  ssageTamperingEr
+00000eb0: 726f 722e 5f5f 696e 6974 5f5f 2905 7217  ror.__init__).r.
+00000ec0: 0000 0072 1800 0000 7219 0000 0072 1100  ...r....r....r..
+00000ed0: 0000 721b 0000 0072 1500 0000 7215 0000  ..r....r....r...
+00000ee0: 0072 1300 0000 7216 0000 0072 5800 0000  .r....r....rX...
+00000ef0: 5700 0000 7302 0000 0008 0172 5800 0000  W...s......rX...
+00000f00: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
+00000f10: 0004 0000 0040 0000 0073 9200 0000 6500  .....@...s....e.
+00000f20: 5a01 6400 5a02 6503 6504 6505 6602 1900  Z.d.Z.e.e.e.f...
+00000f30: 6504 6401 6402 9c03 6403 6404 8404 5a06  e.d.d...d.d...Z.
+00000f40: 6505 6405 9c01 6406 6407 8404 5a07 6508  e.d...d.d...Z.e.
+00000f50: 6405 9c01 6408 6409 8404 5a09 640a 640b  d...d.d...Z.d.d.
+00000f60: 8400 5a0a 640c 640d 8400 5a0b 640e 640f  ..Z.d.d...Z.d.d.
+00000f70: 8400 5a0c 6505 6405 9c01 6410 6411 8404  ..Z.e.d...d.d...
+00000f80: 5a0d 6505 6405 9c01 6412 6413 8404 5a0e  Z.e.d...d.d...Z.
+00000f90: 6505 6405 9c01 6414 6415 8404 5a0f 6504  e.d...d.d...Z.e.
+00000fa0: 6405 9c01 6416 6417 8404 5a10 6401 5300  d...d.d...Z.d.S.
+00000fb0: 2918 da03 4465 634e 721d 0000 0063 0300  )...DecNr....c..
+00000fc0: 0000 0000 0000 0000 0000 0400 0000 0600  ................
+00000fd0: 0000 4300 0000 7306 0100 0074 007c 0174  ..C...s....t.|.t
+00000fe0: 0183 0272 227c 01a0 0264 01a1 017d 0374  ...r"|...d...}.t
+00000ff0: 03a0 047c 03a1 017c 005f 056e 1074 007c  ...|...|._.n.t.|
+00001000: 0174 0683 0272 327c 017c 005f 057c 027c  .t...r2|.|._.|.|
+00001010: 005f 077c 006a 0564 0064 0285 0219 007c  ._.|.j.d.d.....|
+00001020: 005f 087c 006a 0564 0264 0385 0219 007c  ._.|.j.d.d.....|
+00001030: 005f 097c 006a 0564 0364 0485 0219 007c  ._.|.j.d.d.....|
+00001040: 005f 0a7c 006a 0564 0464 0585 0219 007c  ._.|.j.d.d.....|
+00001050: 005f 0b74 0ca0 0d64 067c 006a 0564 0564  ._.t...d.|.j.d.d
+00001060: 0785 0219 00a1 0264 0819 007c 005f 0e7c  .......d...|._.|
+00001070: 006a 0e64 096b 0073 a87c 006a 0e64 0a6b  .j.d.k.s.|.j.d.k
+00001080: 0472 b274 0f7c 006a 0e83 0182 017c 006a  .r.t.|.j.....|.j
+00001090: 0564 0764 0085 0219 007c 005f 1074 11a0  .d.d.....|._.t..
+000010a0: 127c 006a 077c 006a 0a7c 006a 0ea1 037c  .|.j.|.j.|.j...|
+000010b0: 005f 1374 11a0 127c 006a 077c 006a 0b7c  ._.t...|.j.|.j.|
+000010c0: 006a 0ea1 037c 005f 147c 00a0 15a1 0064  .j...|._.|.....d
+000010d0: 0b75 0090 0172 0274 1683 0082 0164 0053  .u...r.t.....d.S
+000010e0: 0029 0c4e 7231 0000 0072 3600 0000 e950  .).Nr1...r6....P
+000010f0: 0000 00e9 6000 0000 e970 0000 0072 4e00  ....`....p...rN.
+00001100: 0000 e974 0000 0072 0100 0000 7221 0000  ...t...r....r!..
+00001110: 0072 2200 0000 4629 1772 2300 0000 7224  .r"...F).r#...r$
+00001120: 0000 0072 2500 0000 7253 0000 005a 1175  ...r%...rS...Z.u
+00001130: 726c 7361 6665 5f62 3634 6465 636f 6465  rlsafe_b64decode
+00001140: 721e 0000 0072 2600 0000 723e 0000 00da  r....r&...r>....
+00001150: 0872 6563 5f68 6d61 63da 0672 6563 5f69  .rec_hmac..rec_i
+00001160: 765a 0872 6563 5f73 616c 745a 0a72 6563  vZ.rec_saltZ.rec
+00001170: 5f70 6570 7065 7272 4f00 0000 5a06 756e  _pepperrO...Z.un
+00001180: 7061 636b 5a0e 7265 635f 6974 6572 6174  packZ.rec_iterat
+00001190: 696f 6e73 720a 0000 00da 0e72 6563 5f63  ionsr......rec_c
+000011a0: 6970 6865 7274 6578 7472 1c00 0000 722d  iphertextr....r-
+000011b0: 0000 00da 0664 6563 4b65 79da 0668 6d61  .....decKey..hma
+000011c0: 635f 6bda 0a76 6572 6966 7948 4d41 4372  c_k..verifyHMACr
+000011d0: 5800 0000 2904 7212 0000 0072 1e00 0000  X...).r....r....
+000011e0: 721f 0000 00da 016d 7215 0000 0072 1500  r......mr....r..
+000011f0: 0000 7216 0000 0072 1100 0000 5e00 0000  ..r....r....^...
+00001200: 732c 0000 0000 010a 010a 010e 010a 0106  s,..............
+00001210: 0106 0110 0110 0110 0110 011c 0114 010a  ................
+00001220: 0110 0116 0104 0104 0104 0104 fd06 040e  ................
+00001230: 017a 0c44 6563 2e5f 5f69 6e69 745f 5f72  .z.Dec.__init__r
+00001240: 3500 0000 6301 0000 0000 0000 0000 0000  5...c...........
+00001250: 0002 0000 0005 0000 0043 0000 0073 2a00  .........C...s*.
+00001260: 0000 7c00 6a00 7d01 7401 a002 7c01 7403  ..|.j.}.t...|.t.
+00001270: a004 a100 a102 7d01 7c01 a005 7c00 6a06  ......}.|...|.j.
+00001280: a101 0100 7c01 a007 a100 5300 7239 0000  ....|.....S.r9..
+00001290: 0029 0872 6200 0000 7208 0000 0072 4a00  .).rb...r....rJ.
+000012a0: 0000 7207 0000 0072 4b00 0000 7246 0000  ..r....rK...rF..
+000012b0: 0072 6000 0000 7247 0000 0072 4c00 0000  .r`...rG...rL...
+000012c0: 7215 0000 0072 1500 0000 7216 0000 00da  r....r....r.....
+000012d0: 0a61 6374 7561 6c48 4d41 4375 0000 0073  .actualHMACu...s
+000012e0: 0800 0000 0001 0601 1001 0c01 7a0e 4465  ............z.De
+000012f0: 632e 6163 7475 616c 484d 4143 6301 0000  c.actualHMACc...
+00001300: 0000 0000 0000 0000 0001 0000 0004 0000  ................
+00001310: 0043 0000 0073 1200 0000 7400 a001 7c00  .C...s....t...|.
+00001320: a002 a100 7c00 6a03 a102 5300 7239 0000  ....|.j...S.r9..
+00001330: 0029 04da 0368 6d63 5a0e 636f 6d70 6172  .)...hmcZ.compar
+00001340: 655f 6469 6765 7374 7265 0000 0072 5e00  e_digestre...r^.
+00001350: 0000 723b 0000 0072 1500 0000 7215 0000  ..r;...r....r...
+00001360: 0072 1600 0000 7263 0000 007b 0000 0073  .r....rc...{...s
+00001370: 0200 0000 0001 7a0e 4465 632e 7665 7269  ......z.Dec.veri
+00001380: 6679 484d 4143 6301 0000 0000 0000 0000  fyHMACc.........
+00001390: 0000 0001 0000 0003 0000 0043 0000 0073  ...........C...s
+000013a0: 0c00 0000 7400 a001 7c00 6a02 a101 5300  ....t...|.j...S.
+000013b0: 7239 0000 0029 0372 0400 0000 723a 0000  r9...).r....r:..
+000013c0: 0072 5f00 0000 723b 0000 0072 1500 0000  .r_...r;...r....
+000013d0: 7215 0000 0072 1600 0000 723c 0000 007e  r....r....r<...~
+000013e0: 0000 0073 0200 0000 0001 7a08 4465 632e  ...s......z.Dec.
+000013f0: 6d6f 6465 6301 0000 0000 0000 0000 0000  modec...........
+00001400: 0001 0000 0005 0000 0043 0000 0073 1e00  .........C...s..
+00001410: 0000 7400 7401 6a02 7c00 6a03 6401 8d01  ..t.t.j.|.j.d...
+00001420: 7c00 a004 a100 7405 8300 6402 8d03 5300  |.....t...d...S.
+00001430: 723d 0000 0029 0672 0200 0000 7203 0000  r=...).r....r...
+00001440: 0072 3f00 0000 7261 0000 0072 3c00 0000  .r?...ra...r<...
+00001450: 7206 0000 0072 3b00 0000 7215 0000 0072  r....r;...r....r
+00001460: 1500 0000 7216 0000 0072 4000 0000 8100  ....r....r@.....
+00001470: 0000 730e 0000 0000 0102 0104 0104 ff04  ..s.............
+00001480: 0206 0104 fc7a 0a44 6563 2e63 6970 6865  .....z.Dec.ciphe
+00001490: 7263 0100 0000 0000 0000 0000 0000 0100  rc..............
+000014a0: 0000 0200 0000 4300 0000 730c 0000 007c  ......C...s....|
+000014b0: 00a0 00a1 00a0 01a1 0053 0072 3900 0000  .........S.r9...
+000014c0: 2902 7240 0000 005a 0964 6563 7279 7074  ).r@...Z.decrypt
+000014d0: 6f72 723b 0000 0072 1500 0000 7215 0000  orr;...r....r...
+000014e0: 0072 1600 0000 da10 6369 7068 6572 5f64  .r......cipher_d
+000014f0: 6563 7279 7074 6f72 8800 0000 7302 0000  ecryptor....s...
+00001500: 0000 017a 1444 6563 2e63 6970 6865 725f  ...z.Dec.cipher_
+00001510: 6465 6372 7970 746f 7263 0100 0000 0000  decryptorc......
+00001520: 0000 0000 0000 0100 0000 0300 0000 4300  ..............C.
+00001530: 0000 731c 0000 007c 00a0 00a1 00a0 017c  ..s....|.......|
+00001540: 006a 02a1 017c 00a0 00a1 00a0 03a1 0017  .j...|..........
+00001550: 0053 0072 3900 0000 2904 7267 0000 0072  .S.r9...).rg...r
+00001560: 4600 0000 7260 0000 0072 4700 0000 723b  F...r`...rG...r;
+00001570: 0000 0072 1500 0000 7215 0000 0072 1600  ...r....r....r..
+00001580: 0000 da11 7072 655f 756e 7061 6464 696e  ....pre_unpaddin
+00001590: 675f 6465 638b 0000 0073 0600 0000 0001  g_dec....s......
+000015a0: 0e01 0aff 7a15 4465 632e 7072 655f 756e  ....z.Dec.pre_un
+000015b0: 7061 6464 696e 675f 6465 6363 0100 0000  padding_decc....
+000015c0: 0000 0000 0000 0000 0200 0000 0400 0000  ................
+000015d0: 4300 0000 7324 0000 0074 00a0 0164 01a1  C...s$...t...d..
+000015e0: 01a0 02a1 007d 017c 01a0 037c 00a0 04a1  .....}.|...|....
+000015f0: 00a1 017c 01a0 05a1 0017 0053 0072 4200  ...|.......S.rB.
+00001600: 0000 2906 7205 0000 0072 4400 0000 da08  ..).r....rD.....
+00001610: 756e 7061 6464 6572 7246 0000 0072 6800  unpadderrF...rh.
+00001620: 0000 7247 0000 0029 0272 1200 0000 7269  ..rG...).r....ri
+00001630: 0000 0072 1500 0000 7215 0000 0072 1600  ...r....r....r..
+00001640: 0000 da0a 756e 7061 6464 6564 5f6d 8f00  ....unpadded_m..
+00001650: 0000 7304 0000 0000 010e 017a 0e44 6563  ..s........z.Dec
+00001660: 2e75 6e70 6164 6465 645f 6d63 0100 0000  .unpadded_mc....
+00001670: 0000 0000 0000 0000 0100 0000 0200 0000  ................
+00001680: 4300 0000 7308 0000 007c 00a0 00a1 0053  C...s....|.....S
+00001690: 0072 3900 0000 2901 726a 0000 0072 3b00  .r9...).rj...r;.
+000016a0: 0000 7215 0000 0072 1500 0000 7216 0000  ..r....r....r...
+000016b0: 00da 0a64 6563 546f 4279 7465 7393 0000  ...decToBytes...
+000016c0: 0073 0200 0000 0001 7a0e 4465 632e 6465  .s......z.Dec.de
+000016d0: 6354 6f42 7974 6573 6301 0000 0000 0000  cToBytesc.......
+000016e0: 0000 0000 0001 0000 0003 0000 0043 0000  .............C..
+000016f0: 0073 0e00 0000 7c00 a000 a100 a001 6401  .s....|.......d.
+00001700: a101 5300 7252 0000 0029 0272 6a00 0000  ..S.rR...).rj...
+00001710: 7254 0000 0072 3b00 0000 7215 0000 0072  rT...r;...r....r
+00001720: 1500 0000 7216 0000 00da 0864 6563 546f  ....r......decTo
+00001730: 5374 7296 0000 0073 0200 0000 0001 7a0c  Str....s......z.
+00001740: 4465 632e 6465 6354 6f53 7472 2911 7217  Dec.decToStr).r.
+00001750: 0000 0072 1800 0000 7219 0000 0072 0900  ...r....r....r..
+00001760: 0000 7224 0000 0072 2600 0000 7211 0000  ..r$...r&...r...
+00001770: 0072 6500 0000 da04 626f 6f6c 7263 0000  .re.....boolrc..
+00001780: 0072 3c00 0000 7240 0000 0072 6700 0000  .r<...r@...rg...
+00001790: 7268 0000 0072 6a00 0000 726b 0000 0072  rh...rj...rk...r
+000017a0: 6c00 0000 7215 0000 0072 1500 0000 7215  l...r....r....r.
+000017b0: 0000 0072 1600 0000 7259 0000 005d 0000  ...r....rY...]..
+000017c0: 0073 1400 0000 0801 1a17 0e06 0e03 0803  .s..............
+000017d0: 0807 0803 0e04 0e04 0e03 7259 0000 0029  ..........rY...)
+000017e0: 165a 2663 7279 7074 6f67 7261 7068 792e  .Z&cryptography.
+000017f0: 6861 7a6d 6174 2e70 7269 6d69 7469 7665  hazmat.primitive
+00001800: 732e 6369 7068 6572 7372 0200 0000 7203  s.ciphersr....r.
+00001810: 0000 0072 0400 0000 5a1e 6372 7970 746f  ...r....Z.crypto
+00001820: 6772 6170 6879 2e68 617a 6d61 742e 7072  graphy.hazmat.pr
+00001830: 696d 6974 6976 6573 7205 0000 005a 1c63  imitivesr....Z.c
+00001840: 7279 7074 6f67 7261 7068 792e 6861 7a6d  ryptography.hazm
+00001850: 6174 2e62 6163 6b65 6e64 7372 0600 0000  at.backendsr....
+00001860: 7207 0000 0072 0800 0000 da06 7479 7069  r....r......typi
+00001870: 6e67 7209 0000 0072 6600 0000 7234 0000  ngr....rf...r4..
+00001880: 0072 5300 0000 724f 0000 0072 2700 0000  .rS...rO...r'...
+00001890: da09 4578 6365 7074 696f 6e72 0a00 0000  ..Exceptionr....
+000018a0: 721c 0000 0072 5800 0000 7259 0000 0072  r....rX...rY...r
+000018b0: 1500 0000 7215 0000 0072 1500 0000 7216  ....r....r....r.
+000018c0: 0000 00da 083c 6d6f 6475 6c65 3e01 0000  .....<module>...
+000018d0: 0073 1a00 0000 1401 0c01 0c01 1001 0c01  .s..............
+000018e0: 0801 0801 0801 0801 0803 1006 0e44 1006  .............D..
```

### Comparing `AshCrypt-1.3.4/AshCrypt/__pycache__/AshCryptGUI.cpython-39.pyc` & `AshCrypt-1.3.5/AshCrypt/__pycache__/AshCryptGUI.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `AshCrypt-1.3.4/AshCrypt/__pycache__/Database.cpython-39.pyc` & `AshCrypt-1.3.5/AshCrypt/__pycache__/Database.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `AshCrypt-1.3.4/AshCrypt/__pycache__/FileCrypt.cpython-39.pyc` & `AshCrypt-1.3.5/AshCrypt/__pycache__/FileCrypt.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `AshCrypt-1.3.4/AshCrypt/__pycache__/TextCrypt.cpython-39.pyc` & `AshCrypt-1.3.5/AshCrypt/__pycache__/TextCrypt.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `AshCrypt-1.3.4/AshCrypt/__pycache__/qr.cpython-39.pyc` & `AshCrypt-1.3.5/AshCrypt/__pycache__/qr.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `AshCrypt-1.3.4/AshCrypt/unittests/__pycache__/unittestAsh.cpython-39.pyc` & `AshCrypt-1.3.5/AshCrypt/unittests/__pycache__/unittestAsh.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `AshCrypt-1.3.4/AshCrypt/unittests/unittestAsh.py` & `AshCrypt-1.3.5/AshCrypt/unittests/unittestAsh.py`

 * *Files identical despite different names*

### Comparing `AshCrypt-1.3.4/AshCrypt.egg-info/PKG-INFO` & `AshCrypt-1.3.5/AshCrypt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AshCrypt
-Version: 1.3.4
+Version: 1.3.5
 Summary: Comprehensive AES-256 Cryptography App & library equipped with files & text handling modules along with a database module to store encrypted content.
 Home-page: https://github.com/AshGw/AES-256.git
 Author: Ashref Gwader
 Author-email: AshrefGw@proton.me
 Keywords: Cryptography application,cryptography libraryAES-256
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `AshCrypt-1.3.4/AshCrypt.egg-info/SOURCES.txt` & `AshCrypt-1.3.5/AshCrypt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `AshCrypt-1.3.4/LICENSE` & `AshCrypt-1.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `AshCrypt-1.3.4/PKG-INFO` & `AshCrypt-1.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AshCrypt
-Version: 1.3.4
+Version: 1.3.5
 Summary: Comprehensive AES-256 Cryptography App & library equipped with files & text handling modules along with a database module to store encrypted content.
 Home-page: https://github.com/AshGw/AES-256.git
 Author: Ashref Gwader
 Author-email: AshrefGw@proton.me
 Keywords: Cryptography application,cryptography libraryAES-256
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `AshCrypt-1.3.4/README.md` & `AshCrypt-1.3.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -4,28 +4,32 @@
 ## Reason Behind It
 In a world where control, surveillance, and privacy violations are increasingly prevalent, the protection of individual freedom becomes crucial. 
 
 As a firm believer in **Freedom** , I have developed a set of tools in Python that leverages the AES-256 algorithm to make it easier for undividuals to safeguard their data without blindly relying on third parties to do it tor them  . 
 
 My aim here is to make these tools accessible and user-friendly, even for individuals with limited programming knowledge. By providing these resources, I hope to contribute to the preservation of privacy and enable individuals to take control of their own data security, so feel free to explore these tools.
 ## Overview ## 
-The project incorporates a library I made called **AshCrypt** : 
+![alt text](important/GUI.png)
+The project incorporates an App & a library called **AshCrypt** : 
+
+**App :** 
+<br>Fully-fledged application that integrates all the modules in the library merging them into a unified and powerful software solution for developers and for people with no programming knowledge whatsoever
+<br>check [GUI](https://github.com/AshGw/AES-256#AshCryptGUI) header for more info.
 
+**Library :** 
 <br>A simple, secure, and developer-oriented library for
 encryption and decryption with AES-256 (CBC) . 
 <br>The core of the library is the module `Ash`
 It offers an intuitive interface, seamless integration with precompiled 
 functions, and robust security measures to safeguard
 sensitive data,  providing a hassle-free experience when dealing with cryptographic libraries.
 <br>View [Features](https://github.com/AshGw/AES-256#features) Header for more details.
 
 
 
-The project mainly includes a fully fledged application that integrates all the modules in the library merging them into a unified and powerful software solution for developers and for people with no programming knowledge whatsoever
-<br>check [GUI](https://github.com/AshGw/AES-256#AshCryptGUI) header for more info.
 
 
 ### For Developers ###
 The project uses `Ash` module to ensure secure data encryption and decryption for Files and Texts while keeping it very easy and simple to use .
 view the headers for [FileCrypt](https://github.com/AshGw/AES-256#filecrypt) and [TextCrypt](https://github.com/AshGw/AES-256#textcrypt) to learn more.
 
 
@@ -182,15 +186,14 @@
 ### Regarding KDFs
 Note that bcrypt is intentionally slow and computationally expensive, enhancing protection against brute-force attacks. The number of iterations, including salt and pepper, increases derivation time to strike a balance between security and performance. Use a suitable value based on your machine's capabilities and desired security level.
 <br>Im using 50 just to demonstrate the process and make it quick.
 <br>The bare minimum is 50, the max is 100 000, choose somewhere in between.
 <br>In my use case 50 takes around 0.5 secs while using the maximum number of iterations takes around 11 minutes to derive the keys and finish the cryptographic operations at hand.
 <br>You can check how it works by checking this [Jupyter Notebook](demo/demo.ipynb) demo file
 ## AshCryptGUI ##
-![alt text](important/GUI.png)
 The GUI as mentioned above is a fully fledged application , you can use it to encrypt files , texts , keep track of files by storing them on demand to a main database , also on demand it can keep track of the keys used for cryptographic operations.
 ### Usage ###
 1) Set the main key up. If you don't have one , press on the button `generate` to generate a secure safe key ready for use. 
 2) Now you're able to encrypt files or text (text is limited to 200 characters max)
 ####  Text : 
 - You can insert some text in the entry right below the `TEXT ENCRYPTION` label.<br>The given text will be encrypted and you can choose if you want to have that text displayed as a qr code, a qr image will pop on the screen and you'll be able to scan it using your phone.
 - Insert some encrypted text below the `TEXT DECRYPTION` label.<br>The Given text will be decrypted and you'd have the option to display the "plaintext" as a qr code to be scanned by other devices.
```

### Comparing `AshCrypt-1.3.4/setup.py` & `AshCrypt-1.3.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup , find_packages
 
 with open('AshCrypt/README.md','r') as f:
     readme = f.read()
 
 setup(
     name='AshCrypt',
-    version='1.3.4',
+    version='1.3.5',
     author='Ashref Gwader',
     author_email='AshrefGw@proton.me',
     python_requires='>=3.7',
     description="Comprehensive AES-256 Cryptography App & library equipped with files & text handling modules along with"
                 " a database module to store encrypted content.",
     long_description_content_type='text/markdown',
     long_description=readme,
```

