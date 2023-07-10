# Comparing `tmp/CTkColorPicker-0.6.0.tar.gz` & `tmp/CTkColorPicker-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CTkColorPicker-0.6.0.tar", last modified: Wed May 17 13:58:11 2023, max compression
+gzip compressed data, was "CTkColorPicker-0.7.0.tar", last modified: Mon Jul 10 07:06:09 2023, max compression
```

## Comparing `CTkColorPicker-0.6.0.tar` & `CTkColorPicker-0.7.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-17 13:58:11.580203 CTkColorPicker-0.6.0/
-drwxrwxrwx   0        0        0        0 2023-05-17 13:58:11.548954 CTkColorPicker-0.6.0/CTkColorPicker/
--rw-rw-rw-   0        0        0      272 2023-05-17 13:38:07.000000 CTkColorPicker-0.6.0/CTkColorPicker/__init__.py
--rw-rw-rw-   0        0        0   111614 2020-05-30 05:51:52.000000 CTkColorPicker-0.6.0/CTkColorPicker/color_wheel.png
--rw-rw-rw-   0        0        0     9081 2023-05-17 13:36:46.000000 CTkColorPicker-0.6.0/CTkColorPicker/ctk_color_picker.py
--rw-rw-rw-   0        0        0     7068 2023-05-17 13:51:56.000000 CTkColorPicker-0.6.0/CTkColorPicker/ctk_color_picker_widget.py
--rw-rw-rw-   0        0        0      933 2020-05-30 05:51:52.000000 CTkColorPicker-0.6.0/CTkColorPicker/target.png
-drwxrwxrwx   0        0        0        0 2023-05-17 13:58:11.564578 CTkColorPicker-0.6.0/CTkColorPicker.egg-info/
--rw-rw-rw-   0        0        0     3653 2023-05-17 13:58:11.000000 CTkColorPicker-0.6.0/CTkColorPicker.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      386 2023-05-17 13:58:11.000000 CTkColorPicker-0.6.0/CTkColorPicker.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       73 2023-05-17 13:58:11.000000 CTkColorPicker-0.6.0/CTkColorPicker.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       21 2023-05-17 13:58:11.000000 CTkColorPicker-0.6.0/CTkColorPicker.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-05-17 13:58:11.000000 CTkColorPicker-0.6.0/CTkColorPicker.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     7048 2022-11-20 16:16:56.000000 CTkColorPicker-0.6.0/LICENSE
--rw-rw-rw-   0        0        0     3653 2023-05-17 13:58:11.580203 CTkColorPicker-0.6.0/PKG-INFO
--rw-rw-rw-   0        0        0     2974 2023-05-17 13:55:59.000000 CTkColorPicker-0.6.0/README.md
--rw-rw-rw-   0        0        0      607 2023-05-17 13:58:11.580203 CTkColorPicker-0.6.0/setup.cfg
--rw-rw-rw-   0        0        0     1317 2023-05-17 13:54:31.000000 CTkColorPicker-0.6.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-10 07:06:09.873749 CTkColorPicker-0.7.0/
+drwxrwxrwx   0        0        0        0 2023-07-10 07:06:09.853856 CTkColorPicker-0.7.0/CTkColorPicker/
+-rw-rw-rw-   0        0        0      272 2023-07-10 07:04:41.000000 CTkColorPicker-0.7.0/CTkColorPicker/__init__.py
+-rw-rw-rw-   0        0        0   111614 2020-05-30 05:51:52.000000 CTkColorPicker-0.7.0/CTkColorPicker/color_wheel.png
+-rw-rw-rw-   0        0        0     9267 2023-07-10 07:02:57.000000 CTkColorPicker-0.7.0/CTkColorPicker/ctk_color_picker.py
+-rw-rw-rw-   0        0        0     7220 2023-07-10 07:01:48.000000 CTkColorPicker-0.7.0/CTkColorPicker/ctk_color_picker_widget.py
+-rw-rw-rw-   0        0        0      933 2020-05-30 05:51:52.000000 CTkColorPicker-0.7.0/CTkColorPicker/target.png
+drwxrwxrwx   0        0        0        0 2023-07-10 07:06:09.863804 CTkColorPicker-0.7.0/CTkColorPicker.egg-info/
+-rw-rw-rw-   0        0        0     3653 2023-07-10 07:06:09.000000 CTkColorPicker-0.7.0/CTkColorPicker.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      386 2023-07-10 07:06:09.000000 CTkColorPicker-0.7.0/CTkColorPicker.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       73 2023-07-10 07:06:09.000000 CTkColorPicker-0.7.0/CTkColorPicker.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       21 2023-07-10 07:06:09.000000 CTkColorPicker-0.7.0/CTkColorPicker.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-07-10 07:06:09.000000 CTkColorPicker-0.7.0/CTkColorPicker.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     7048 2022-11-20 16:16:56.000000 CTkColorPicker-0.7.0/LICENSE
+-rw-rw-rw-   0        0        0     3653 2023-07-10 07:06:09.873749 CTkColorPicker-0.7.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2974 2023-05-17 13:55:59.000000 CTkColorPicker-0.7.0/README.md
+-rw-rw-rw-   0        0        0      607 2023-07-10 07:06:09.873749 CTkColorPicker-0.7.0/setup.cfg
+-rw-rw-rw-   0        0        0     1317 2023-07-10 07:05:39.000000 CTkColorPicker-0.7.0/setup.py
```

### Comparing `CTkColorPicker-0.6.0/CTkColorPicker/color_wheel.png` & `CTkColorPicker-0.7.0/CTkColorPicker/color_wheel.png`

 * *Files identical despite different names*

### Comparing `CTkColorPicker-0.6.0/CTkColorPicker/ctk_color_picker.py` & `CTkColorPicker-0.7.0/CTkColorPicker/ctk_color_picker.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,15 +15,15 @@
         ctypes.windll.shcore.SetProcessDpiAwareness(0)
     except:
         pass
 
 PATH = os.path.dirname(os.path.realpath(__file__))
 
 class AskColor(customtkinter.CTkToplevel):
-    
+
     def __init__(self,
                  width: int = 300,
                  title: str = "Choose Color",
                  initial_color: str = None,
                  bg_color: str = None,
                  fg_color: str = None,
                  button_color: str = None,
@@ -108,19 +108,27 @@
         self.master.wait_window(self)
         return self._color
     
     def _ok_event(self, event=None):
         self._color = self.label._fg_color
         self.grab_release()
         self.destroy()
+        del self.img1
+        del self.img2
+        del self.wheel
+        del self.target
         
     def _on_closing(self):
         self._color = None
         self.grab_release()
         self.destroy()
+        del self.img1
+        del self.img2
+        del self.wheel
+        del self.target
         
     def on_mouse_drag(self, event):
         x = event.x
         y = event.y
         self.canvas.delete("all")
         self.canvas.create_image(self.image_dimension/2, self.image_dimension/2, image=self.wheel)
```

### Comparing `CTkColorPicker-0.6.0/CTkColorPicker/ctk_color_picker_widget.py` & `CTkColorPicker-0.7.0/CTkColorPicker/ctk_color_picker_widget.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,14 +76,21 @@
         self.label = customtkinter.CTkLabel(master=self, text_color="#000000", width=10, fg_color=self.default_hex_color,
                                             corner_radius=self.corner_radius, text=self.default_hex_color, wraplength=1)
         self.label.pack(expand=True, fill="both", padx=10, pady=15)
         
     def get(self):
         self._color = self.label._fg_color
         return self._color
+    
+    def destroy(self):
+        super().destroy()
+        del self.img1
+        del self.img2
+        del self.wheel
+        del self.target
         
     def on_mouse_drag(self, event):
         x = event.x
         y = event.y
         self.canvas.delete("all")
         self.canvas.create_image(self.image_dimension/2, self.image_dimension/2, image=self.wheel)
```

### Comparing `CTkColorPicker-0.6.0/CTkColorPicker/target.png` & `CTkColorPicker-0.7.0/CTkColorPicker/target.png`

 * *Files identical despite different names*

### Comparing `CTkColorPicker-0.6.0/CTkColorPicker.egg-info/PKG-INFO` & `CTkColorPicker-0.7.0/CTkColorPicker.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CTkColorPicker
-Version: 0.6.0
+Version: 0.7.0
 Summary: A modern color picker for customtkinter
 Home-page: https://github.com/Akascape/CTkColorPicker
 Author: Akash Bora
 License: Creative Commons Zero v1.0 Universal
 Keywords: customtkinter,customtkinter-dialog,customtkinter-color-picker,customtkinter-colour-picker,customtkinter-color,customtkinter-color-chooser,color-picker,python-color-picker
 Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
 Classifier: Programming Language :: Python :: 3
```

### Comparing `CTkColorPicker-0.6.0/LICENSE` & `CTkColorPicker-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `CTkColorPicker-0.6.0/PKG-INFO` & `CTkColorPicker-0.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CTkColorPicker
-Version: 0.6.0
+Version: 0.7.0
 Summary: A modern color picker for customtkinter
 Home-page: https://github.com/Akascape/CTkColorPicker
 Author: Akash Bora
 License: Creative Commons Zero v1.0 Universal
 Keywords: customtkinter,customtkinter-dialog,customtkinter-color-picker,customtkinter-colour-picker,customtkinter-color,customtkinter-color-chooser,color-picker,python-color-picker
 Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
 Classifier: Programming Language :: Python :: 3
```

### Comparing `CTkColorPicker-0.6.0/README.md` & `CTkColorPicker-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `CTkColorPicker-0.6.0/setup.cfg` & `CTkColorPicker-0.7.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2043 546b 436f 6c6f 7250 6963 6b65   = CTkColorPicke
-00000020: 720d 0a76 6572 7369 6f6e 203d 2030 2e36  r..version = 0.6
+00000020: 720d 0a76 6572 7369 6f6e 203d 2030 2e37  r..version = 0.7
 00000030: 2e30 0d0a 6465 7363 7269 7074 696f 6e20  .0..description 
 00000040: 3d20 4120 6d6f 6465 726e 2063 6f6c 6f72  = A modern color
 00000050: 2070 6963 6b65 7220 666f 7220 6375 7374   picker for cust
 00000060: 6f6d 746b 696e 7465 720d 0a6c 6f6e 675f  omtkinter..long_
 00000070: 6465 7363 7269 7074 696f 6e20 3d20 6669  description = fi
 00000080: 6c65 3a20 5245 4144 4d45 2e6d 640d 0a6c  le: README.md..l
 00000090: 6f6e 675f 6465 7363 7269 7074 696f 6e5f  ong_description_
```

### Comparing `CTkColorPicker-0.6.0/setup.py` & `CTkColorPicker-0.7.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     """Opens and fetches text of long descrition file."""
     with open(path, 'r') as f:
         text = f.read()
     return text
 
 setup(
     name = 'CTkColorPicker',
-    version = '0.6.0',
+    version = '0.7.0',
     description = "A modern color picker for customtkinter",
     license = "Creative Commons Zero v1.0 Universal",
     readme = "README.md",
     long_description = get_long_description('README.md'),
     long_description_content_type = "text/markdown",
     author = 'Akash Bora',
     url = "https://github.com/Akascape/CTkColorPicker",
```

