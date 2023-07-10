# Comparing `tmp/CTkListbox-0.2.tar.gz` & `tmp/CTkListbox-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CTkListbox-0.2.tar", last modified: Thu Jul  6 12:25:06 2023, max compression
+gzip compressed data, was "CTkListbox-0.3.tar", last modified: Mon Jul 10 16:29:18 2023, max compression
```

## Comparing `CTkListbox-0.2.tar` & `CTkListbox-0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-06 12:25:06.937996 CTkListbox-0.2/
-drwxrwxrwx   0        0        0        0 2023-07-06 12:25:06.922372 CTkListbox-0.2/CTkListbox/
--rw-rw-rw-   0        0        0      190 2023-06-23 06:27:38.000000 CTkListbox-0.2/CTkListbox/__init__.py
--rw-rw-rw-   0        0        0     5992 2023-06-23 06:33:52.000000 CTkListbox-0.2/CTkListbox/ctk_listbox.py
-drwxrwxrwx   0        0        0        0 2023-07-06 12:25:06.937996 CTkListbox-0.2/CTkListbox.egg-info/
--rw-rw-rw-   0        0        0     2764 2023-07-06 12:25:06.000000 CTkListbox-0.2/CTkListbox.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      254 2023-07-06 12:25:06.000000 CTkListbox-0.2/CTkListbox.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       40 2023-07-06 12:25:06.000000 CTkListbox-0.2/CTkListbox.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-07-06 12:25:06.000000 CTkListbox-0.2/CTkListbox.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-07-06 12:25:06.000000 CTkListbox-0.2/CTkListbox.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1067 2023-06-21 11:17:36.000000 CTkListbox-0.2/LICENSE
--rw-rw-rw-   0        0        0     2764 2023-07-06 12:25:06.937996 CTkListbox-0.2/PKG-INFO
--rw-rw-rw-   0        0        0     2187 2023-07-06 12:24:22.000000 CTkListbox-0.2/README.md
--rw-rw-rw-   0        0        0      527 2023-07-06 12:25:06.937996 CTkListbox-0.2/setup.cfg
--rw-rw-rw-   0        0        0     1042 2023-07-06 12:22:17.000000 CTkListbox-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-10 16:29:18.140320 CTkListbox-0.3/
+drwxrwxrwx   0        0        0        0 2023-07-10 16:29:18.073315 CTkListbox-0.3/CTkListbox/
+-rw-rw-rw-   0        0        0      190 2023-07-10 16:27:56.000000 CTkListbox-0.3/CTkListbox/__init__.py
+-rw-rw-rw-   0        0        0     6599 2023-07-10 16:26:42.000000 CTkListbox-0.3/CTkListbox/ctk_listbox.py
+drwxrwxrwx   0        0        0        0 2023-07-10 16:29:18.137319 CTkListbox-0.3/CTkListbox.egg-info/
+-rw-rw-rw-   0        0        0     2764 2023-07-10 16:29:17.000000 CTkListbox-0.3/CTkListbox.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      254 2023-07-10 16:29:18.000000 CTkListbox-0.3/CTkListbox.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       40 2023-07-10 16:29:17.000000 CTkListbox-0.3/CTkListbox.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-07-10 16:29:17.000000 CTkListbox-0.3/CTkListbox.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-10 16:29:17.000000 CTkListbox-0.3/CTkListbox.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1067 2023-06-21 11:17:36.000000 CTkListbox-0.3/LICENSE
+-rw-rw-rw-   0        0        0     2764 2023-07-10 16:29:18.140320 CTkListbox-0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2187 2023-07-06 12:24:22.000000 CTkListbox-0.3/README.md
+-rw-rw-rw-   0        0        0      527 2023-07-10 16:29:18.146322 CTkListbox-0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1042 2023-07-10 16:28:10.000000 CTkListbox-0.3/setup.py
```

### Comparing `CTkListbox-0.2/CTkListbox/ctk_listbox.py` & `CTkListbox-0.3/CTkListbox/ctk_listbox.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,32 +18,40 @@
                  select_color: str = "default",
                  hover_color: str = "default",
                  border_width: int = 3,
                  font: tuple = "default",
                  multiple_selection: bool = False,
                  hover: bool = True,
                  command = None,
+                 justify = "left",
                  **kwargs):
         
         super().__init__(master, width=width, height=height, fg_color=fg_color, border_width=border_width, **kwargs)
         self._scrollbar.grid_configure(padx=(0,border_width))
         self._scrollbar.configure(width=12)
         
         if bg_color:
             super().configure(bg_color=bg_color)
-
+        
         self.select_color = customtkinter.ThemeManager.theme["CTkButton"]["fg_color"] if select_color=="default" else select_color
         self.text_color = customtkinter.ThemeManager.theme["CTkButton"]["text_color"] if text_color=="default" else text_color
         self.hover_color = customtkinter.ThemeManager.theme["CTkButton"]["hover_color"] if hover_color=="default" else hover_color
         self.font = (customtkinter.ThemeManager.theme["CTkFont"]["family"],13) if font=="default" else font
+        if justify=="left":
+            self.justify = "w"
+        elif justify=="right":
+            self.justify = "e"
+        else:
+            self.justify = "c"
         self.buttons = {}
         self.command = command
         self.multiple = multiple_selection
         self.selected = None
         self.hover = hover
+        self.end_num = 0 
         self.selections = []
     
     def select(self, index):
         """ select the option """
         for options in self.buttons.values():
             options.configure(fg_color="transparent")
         
@@ -61,55 +69,62 @@
             self.selected = self.buttons[index]
             self.buttons[index].configure(fg_color=self.select_color, hover=False)
             self.after(100, lambda: self.buttons[index].configure(hover=self.hover))
             
         if self.command:
             self.command(self.get())
             
+    def bind(self, key, func):
+        super().bind_all(key, lambda e: func(self.get()))
+        
     def deselect(self, index):
         if not self.multiple:
             self.selected.configure(fg_color="transparent")
             self.selected = None
             return
         if self.buttons[index] in self.selections:
             self.selections.remove(self.buttons[index])
             self.buttons[index].configure(fg_color="transparent")
        
-    def insert(self, index, option, justify="left", **args):
-        """ select new value in the listbox """
-        if justify=="left":
-            justify = "w"
-        elif justify=="right":
-            justify = "e"
-        else:
-            justify = "c"
+    def insert(self, index, option, **args):
+        """ add new option in the listbox """
+                
+        if str(index).lower()=="end":
+            index = f"END{self.end_num}"
+            self.end_num +=1
             
-        if index in self.buttons:
-            if index!="END":
-                self.delete(index)
-            
-        self.buttons[index] = customtkinter.CTkButton(self, text=option, fg_color="transparent", anchor=justify,
+        self.buttons[index] = customtkinter.CTkButton(self, text=option, fg_color="transparent", anchor=self.justify,
                                                       text_color=self.text_color, font=self.font,
                                                       hover_color=self.hover_color, **args)
         self.buttons[index].configure(command=lambda num=index: self.select(num))
         self.buttons[index].pack(padx=0, pady=(0,5), fill="x", expand=True)
 
     def delete(self, index):
-        """ delete a value from the listbox """
+        """ delete a option from the listbox """
+        if str(index).lower()=="end":
+            index = f"END{self.end_num}"
+            self.end_num -=1
+
+        if str(index).lower()=="all":
+            for i in self.buttons:
+                self.buttons[i].destroy()
+            self.buttons = {}
+            self.end_num = 0
+            return
         self.buttons[index].destroy()
         del self.buttons[index]
         
     def size(self):
         """ return total number of items in the listbox """
         return len(self.buttons.values())
 
     def get(self, index=None):
         """ get the selected value """
         if index:
-            if index=="ALL":
+            if str(index).lower=="all":
                 return self.buttons[index].cget("text")
             else:
                 return list(item.cget("text") for item in self.buttons.values())
         else:
             if self.multiple:
                 return [x.cget("text") for x in self.selections] if len(self.selections)>0 else None
             else:
@@ -132,9 +147,11 @@
             self.text_color = kwargs.pop("text_color")
             for i in self.buttons.values():
                 i.configure(text=self.text_color)
         if "font" in kwargs:
             self.font = kwargs.pop("font")
             for i in self.buttons.values():
                 i.configure(font=self.font)
-
+        if "command" in kwargs:
+            self.command = kwargs.pop("command")
+            
         super().configure(**kwargs)
```

### Comparing `CTkListbox-0.2/CTkListbox.egg-info/PKG-INFO` & `CTkListbox-0.3/CTkListbox.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CTkListbox
-Version: 0.2
+Version: 0.3
 Summary: Customtkinter Listbox widget
 Home-page: https://github.com/Akascape/CTkListbox
 Author: Akash Bora
 License: MIT
 Keywords: customtkinter,tkinter,listbox-widget,listbox,modern-listbox,option menu,list-box
 Classifier: License :: OSI Approved :: MIT License 
 Classifier: Programming Language :: Python :: 3
```

### Comparing `CTkListbox-0.2/LICENSE` & `CTkListbox-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `CTkListbox-0.2/PKG-INFO` & `CTkListbox-0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CTkListbox
-Version: 0.2
+Version: 0.3
 Summary: Customtkinter Listbox widget
 Home-page: https://github.com/Akascape/CTkListbox
 Author: Akash Bora
 License: MIT
 Keywords: customtkinter,tkinter,listbox-widget,listbox,modern-listbox,option menu,list-box
 Classifier: License :: OSI Approved :: MIT License 
 Classifier: Programming Language :: Python :: 3
```

### Comparing `CTkListbox-0.2/README.md` & `CTkListbox-0.3/README.md`

 * *Files identical despite different names*

### Comparing `CTkListbox-0.2/setup.cfg` & `CTkListbox-0.3/setup.cfg`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2043 546b 4c69 7374 626f 780d 0a76   = CTkListbox..v
-00000020: 6572 7369 6f6e 203d 2030 2e32 0d0a 6465  ersion = 0.2..de
+00000020: 6572 7369 6f6e 203d 2030 2e33 0d0a 6465  ersion = 0.3..de
 00000030: 7363 7269 7074 696f 6e20 3d20 4375 7374  scription = Cust
 00000040: 6f6d 746b 696e 7465 7220 4c69 7374 626f  omtkinter Listbo
 00000050: 7820 7769 6467 6574 0d0a 6c6f 6e67 5f64  x widget..long_d
 00000060: 6573 6372 6970 7469 6f6e 203d 2066 696c  escription = fil
 00000070: 653a 2052 4541 444d 452e 6d64 0d0a 6c6f  e: README.md..lo
 00000080: 6e67 5f64 6573 6372 6970 7469 6f6e 5f63  ng_description_c
 00000090: 6f6e 7465 6e74 5f74 7970 6520 3d20 7465  ontent_type = te
```

### Comparing `CTkListbox-0.2/setup.py` & `CTkListbox-0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     """Opens and fetches text of long descrition file."""
     with open(path, 'r') as f:
         text = f.read()
     return text
 
 setup(
     name = 'CTkListbox',
-    version = '0.2',
+    version = '0.3',
     description = "Customtkinter Listbox widget",
     license = "MIT",
     readme = "README.md",
     long_description = get_long_description('README.md'),
     long_description_content_type = "text/markdown",
     author = 'Akash Bora',
     url = "https://github.com/Akascape/CTkListbox",
```

