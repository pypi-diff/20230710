# Comparing `tmp/CTkMessagebox-2.1.tar.gz` & `tmp/CTkMessagebox-2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CTkMessagebox-2.1.tar", last modified: Sat Jul  8 07:27:14 2023, max compression
+gzip compressed data, was "CTkMessagebox-2.2.tar", last modified: Mon Jul 10 06:17:45 2023, max compression
```

## Comparing `CTkMessagebox-2.1.tar` & `CTkMessagebox-2.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-07-08 07:27:14.185962 CTkMessagebox-2.1/
-drwxrwxrwx   0        0        0        0 2023-07-08 07:27:14.170336 CTkMessagebox-2.1/CTkMessagebox/
--rw-rw-rw-   0        0        0      232 2023-07-08 07:24:55.000000 CTkMessagebox-2.1/CTkMessagebox/__init__.py
--rw-rw-rw-   0        0        0    14359 2023-07-08 07:23:07.000000 CTkMessagebox-2.1/CTkMessagebox/ctkmessagebox.py
-drwxrwxrwx   0        0        0        0 2023-07-08 07:27:14.185962 CTkMessagebox-2.1/CTkMessagebox/icons/
--rw-rw-rw-   0        0        0    38437 2023-02-24 17:58:14.000000 CTkMessagebox-2.1/CTkMessagebox/icons/cancel.png
--rw-rw-rw-   0        0        0    31308 2023-02-24 17:40:20.000000 CTkMessagebox-2.1/CTkMessagebox/icons/check.png
--rw-rw-rw-   0        0        0    14921 2023-02-24 18:08:36.000000 CTkMessagebox-2.1/CTkMessagebox/icons/info.png
--rw-rw-rw-   0        0        0    15030 2023-04-14 12:27:30.000000 CTkMessagebox-2.1/CTkMessagebox/icons/question.png
--rw-rw-rw-   0        0        0    17104 2023-02-24 18:03:33.000000 CTkMessagebox-2.1/CTkMessagebox/icons/warning.png
-drwxrwxrwx   0        0        0        0 2023-07-08 07:27:14.185962 CTkMessagebox-2.1/CTkMessagebox.egg-info/
--rw-rw-rw-   0        0        0     7104 2023-07-08 07:27:14.000000 CTkMessagebox-2.1/CTkMessagebox.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      432 2023-07-08 07:27:14.000000 CTkMessagebox-2.1/CTkMessagebox.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       73 2023-07-08 07:27:14.000000 CTkMessagebox-2.1/CTkMessagebox.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       21 2023-07-08 07:27:14.000000 CTkMessagebox-2.1/CTkMessagebox.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-07-08 07:27:14.000000 CTkMessagebox-2.1/CTkMessagebox.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     7048 2022-11-20 16:16:56.000000 CTkMessagebox-2.1/LICENSE
--rw-rw-rw-   0        0        0     7104 2023-07-08 07:27:14.185962 CTkMessagebox-2.1/PKG-INFO
--rw-rw-rw-   0        0        0     6406 2023-07-08 07:24:42.000000 CTkMessagebox-2.1/README.md
--rw-rw-rw-   0        0        0      625 2023-07-08 07:27:14.185962 CTkMessagebox-2.1/setup.cfg
--rw-rw-rw-   0        0        0     1361 2023-07-08 07:25:32.000000 CTkMessagebox-2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-10 06:17:45.256214 CTkMessagebox-2.2/
+drwxrwxrwx   0        0        0        0 2023-07-10 06:17:45.226214 CTkMessagebox-2.2/CTkMessagebox/
+-rw-rw-rw-   0        0        0      232 2023-07-10 06:13:56.000000 CTkMessagebox-2.2/CTkMessagebox/__init__.py
+-rw-rw-rw-   0        0        0    14935 2023-07-10 06:12:40.000000 CTkMessagebox-2.2/CTkMessagebox/ctkmessagebox.py
+drwxrwxrwx   0        0        0        0 2023-07-10 06:17:45.256214 CTkMessagebox-2.2/CTkMessagebox/icons/
+-rw-rw-rw-   0        0        0    38437 2023-02-24 17:58:14.000000 CTkMessagebox-2.2/CTkMessagebox/icons/cancel.png
+-rw-rw-rw-   0        0        0    31308 2023-02-24 17:40:20.000000 CTkMessagebox-2.2/CTkMessagebox/icons/check.png
+-rw-rw-rw-   0        0        0    14921 2023-02-24 18:08:36.000000 CTkMessagebox-2.2/CTkMessagebox/icons/info.png
+-rw-rw-rw-   0        0        0    15030 2023-04-14 12:27:30.000000 CTkMessagebox-2.2/CTkMessagebox/icons/question.png
+-rw-rw-rw-   0        0        0    17104 2023-02-24 18:03:33.000000 CTkMessagebox-2.2/CTkMessagebox/icons/warning.png
+drwxrwxrwx   0        0        0        0 2023-07-10 06:17:45.245962 CTkMessagebox-2.2/CTkMessagebox.egg-info/
+-rw-rw-rw-   0        0        0     7104 2023-07-10 06:17:45.000000 CTkMessagebox-2.2/CTkMessagebox.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      432 2023-07-10 06:17:45.000000 CTkMessagebox-2.2/CTkMessagebox.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       73 2023-07-10 06:17:45.000000 CTkMessagebox-2.2/CTkMessagebox.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       21 2023-07-10 06:17:45.000000 CTkMessagebox-2.2/CTkMessagebox.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-07-10 06:17:45.000000 CTkMessagebox-2.2/CTkMessagebox.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     7048 2022-11-20 16:16:56.000000 CTkMessagebox-2.2/LICENSE
+-rw-rw-rw-   0        0        0     7104 2023-07-10 06:17:45.256214 CTkMessagebox-2.2/PKG-INFO
+-rw-rw-rw-   0        0        0     6406 2023-07-08 07:24:42.000000 CTkMessagebox-2.2/README.md
+-rw-rw-rw-   0        0        0      625 2023-07-10 06:17:45.256214 CTkMessagebox-2.2/setup.cfg
+-rw-rw-rw-   0        0        0     1361 2023-07-10 06:14:15.000000 CTkMessagebox-2.2/setup.py
```

### Comparing `CTkMessagebox-2.1/CTkMessagebox/ctkmessagebox.py` & `CTkMessagebox-2.2/CTkMessagebox/ctkmessagebox.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,28 @@
 """
 CustomTkinter Messagebox
 Author: Akash Bora
-Version: 2.1
+Version: 2.2
 """
 
 import customtkinter
 from PIL import Image
 import os
 import sys
 import time
 
 class CTkMessagebox(customtkinter.CTkToplevel):
-    
+    ICONS = {
+        "check": None,
+        "cancel": None,
+        "info": None,
+        "question": None,
+        "warning": None
+    }
+
     def __init__(self,
                  master: any = None,
                  width: int = 400,
                  height: int = 200,
                  title: str = "CTkMessagebox",
                  message: str = "This is a CTkMessagebox!",
                  option_1: str = "OK",
@@ -173,20 +180,15 @@
             
         if icon_size:
             self.size_height = icon_size[1] if icon_size[1]<=self.height-100 else self.height-100
             self.size = (icon_size[0], self.size_height)
         else:
             self.size = (self.height/4, self.height/4)
         
-        if icon in ["check", "cancel", "info", "question", "warning"]:
-            self.icon = customtkinter.CTkImage(Image.open(os.path.join(os.path.dirname(os.path.realpath(__file__)), 'icons', icon+'.png')),
-                                               size=self.size)
-        else:
-            self.icon = customtkinter.CTkImage(Image.open(icon), size=self.size) if icon else None
-
+        self.icon = self.load_icon(icon, icon_size) if icon else None
         self.frame_top = customtkinter.CTkFrame(self, corner_radius=self.round_corners, width=self.width, border_width=self.border_width,
                                                 bg_color=self.transparent_color, fg_color=self.bg_color, border_color=self.border_color)
         self.frame_top.grid(sticky="nswe")
 
         if button_width:
             self.frame_top.grid_columnconfigure(0, weight=1)
         else:
@@ -254,14 +256,28 @@
             self.frame_top.configure(corner_radius=0)
 
         if self.winfo_exists():
             self.grab_set()
             
         if self.fade:
             self.fade_in()
+            
+    def load_icon(self, icon, icon_size):
+        if icon not in self.ICONS or self.ICONS[icon] is None:
+            if icon in ["check", "cancel", "info", "question", "warning"]:
+                image_path = os.path.join(os.path.dirname(os.path.realpath(__file__)), 'icons', icon + '.png')
+            else:
+                image_path = icon
+            if icon_size:
+                size_height = icon_size[1] if icon_size[1] <= self.height - 100 else self.height - 100
+                size = (icon_size[0], size_height)
+            else:
+                size = (self.height / 4, self.height / 4)
+            self.ICONS[icon] = customtkinter.CTkImage(Image.open(image_path), size=size)
+        return self.ICONS[icon]
         
     def fade_in(self):
         for i in range(0,110,10):
             if not self.winfo_exists():
                 break
             self.attributes("-alpha", i/100)
             self.update()
@@ -297,12 +313,12 @@
         except AttributeError:
             pass
 
         if self.fade:
             self.fade_out()
         self.grab_release()
         self.destroy()
-        self.event = event
-
+        self.event = event  
+        
 if __name__ == "__main__":
     app = CTkMessagebox()
     app.mainloop()
```

### Comparing `CTkMessagebox-2.1/CTkMessagebox/icons/cancel.png` & `CTkMessagebox-2.2/CTkMessagebox/icons/cancel.png`

 * *Files identical despite different names*

### Comparing `CTkMessagebox-2.1/CTkMessagebox/icons/check.png` & `CTkMessagebox-2.2/CTkMessagebox/icons/check.png`

 * *Files identical despite different names*

### Comparing `CTkMessagebox-2.1/CTkMessagebox/icons/info.png` & `CTkMessagebox-2.2/CTkMessagebox/icons/info.png`

 * *Files identical despite different names*

### Comparing `CTkMessagebox-2.1/CTkMessagebox/icons/question.png` & `CTkMessagebox-2.2/CTkMessagebox/icons/question.png`

 * *Files identical despite different names*

### Comparing `CTkMessagebox-2.1/CTkMessagebox/icons/warning.png` & `CTkMessagebox-2.2/CTkMessagebox/icons/warning.png`

 * *Files identical despite different names*

### Comparing `CTkMessagebox-2.1/CTkMessagebox.egg-info/PKG-INFO` & `CTkMessagebox-2.2/CTkMessagebox.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CTkMessagebox
-Version: 2.1
+Version: 2.2
 Summary: A modern messagebox for customtkinter
 Home-page: https://github.com/Akascape/CTkMessagebox
 Author: Akash Bora
 License: Creative Commons Zero v1.0 Universal
 Keywords: customtkinter,customtkinter-dialog,customtkinter-messagebox,customtkinter-message-box,tkinter-messagebox,customtkinter-tkinter-messagebox,messagebox-widget,modern-tkinter-messagebox,ctkmessagebox
 Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: CTkMessagebox Version: 2.1 Summary: A modern
+Metadata-Version: 2.1 Name: CTkMessagebox Version: 2.2 Summary: A modern
 messagebox for customtkinter Home-page: https://github.com/Akascape/
 CTkMessagebox Author: Akash Bora License: Creative Commons Zero v1.0 Universal
 Keywords: customtkinter,customtkinter-dialog,customtkinter-
 messagebox,customtkinter-message-box,tkinter-messagebox,customtkinter-tkinter-
 messagebox,messagebox-widget,modern-tkinter-messagebox,ctkmessagebox
 Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
 Classifier: Programming Language :: Python :: 3 Classifier: Operating System ::
```

### Comparing `CTkMessagebox-2.1/LICENSE` & `CTkMessagebox-2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `CTkMessagebox-2.1/PKG-INFO` & `CTkMessagebox-2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CTkMessagebox
-Version: 2.1
+Version: 2.2
 Summary: A modern messagebox for customtkinter
 Home-page: https://github.com/Akascape/CTkMessagebox
 Author: Akash Bora
 License: Creative Commons Zero v1.0 Universal
 Keywords: customtkinter,customtkinter-dialog,customtkinter-messagebox,customtkinter-message-box,tkinter-messagebox,customtkinter-tkinter-messagebox,messagebox-widget,modern-tkinter-messagebox,ctkmessagebox
 Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: CTkMessagebox Version: 2.1 Summary: A modern
+Metadata-Version: 2.1 Name: CTkMessagebox Version: 2.2 Summary: A modern
 messagebox for customtkinter Home-page: https://github.com/Akascape/
 CTkMessagebox Author: Akash Bora License: Creative Commons Zero v1.0 Universal
 Keywords: customtkinter,customtkinter-dialog,customtkinter-
 messagebox,customtkinter-message-box,tkinter-messagebox,customtkinter-tkinter-
 messagebox,messagebox-widget,modern-tkinter-messagebox,ctkmessagebox
 Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
 Classifier: Programming Language :: Python :: 3 Classifier: Operating System ::
```

### Comparing `CTkMessagebox-2.1/README.md` & `CTkMessagebox-2.2/README.md`

 * *Files identical despite different names*

### Comparing `CTkMessagebox-2.1/setup.cfg` & `CTkMessagebox-2.2/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2043 546b 4d65 7373 6167 6562 6f78   = CTkMessagebox
-00000020: 0d0a 7665 7273 696f 6e20 3d20 322e 310d  ..version = 2.1.
+00000020: 0d0a 7665 7273 696f 6e20 3d20 322e 320d  ..version = 2.2.
 00000030: 0a64 6573 6372 6970 7469 6f6e 203d 2041  .description = A
 00000040: 206d 6f64 6572 6e20 6d65 7373 6167 6562   modern messageb
 00000050: 6f78 2066 6f72 2063 7573 746f 6d74 6b69  ox for customtki
 00000060: 6e74 6572 0d0a 6c6f 6e67 5f64 6573 6372  nter..long_descr
 00000070: 6970 7469 6f6e 203d 2066 696c 653a 2052  iption = file: R
 00000080: 4541 444d 452e 6d64 0d0a 6c6f 6e67 5f64  EADME.md..long_d
 00000090: 6573 6372 6970 7469 6f6e 5f63 6f6e 7465  escription_conte
```

### Comparing `CTkMessagebox-2.1/setup.py` & `CTkMessagebox-2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     """Opens and fetches text of long descrition file."""
     with open(path, 'r') as f:
         text = f.read()
     return text
 
 setup(
     name = 'CTkMessagebox',
-    version = '2.1',
+    version = '2.2',
     description = "A modern messagebox for customtkinter",
     license = "Creative Commons Zero v1.0 Universal",
     readme = "README.md",
     long_description = get_long_description('README.md'),
     long_description_content_type = "text/markdown",
     author = 'Akash Bora',
     url = "https://github.com/Akascape/CTkMessagebox",
```

