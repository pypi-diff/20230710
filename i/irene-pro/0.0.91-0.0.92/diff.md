# Comparing `tmp/irene_pro-0.0.91.tar.gz` & `tmp/irene_pro-0.0.92.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "irene_pro-0.0.91.tar", last modified: Sun Jul  9 08:44:24 2023, max compression
+gzip compressed data, was "irene_pro-0.0.92.tar", last modified: Mon Jul 10 07:03:29 2023, max compression
```

## Comparing `irene_pro-0.0.91.tar` & `irene_pro-0.0.92.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-07-09 08:44:24.192176 irene_pro-0.0.91/
--rw-rw-rw-   0        0        0      227 2023-06-30 07:10:26.000000 irene_pro-0.0.91/LICENSE
--rw-rw-rw-   0        0        0       14 2023-06-30 07:10:26.000000 irene_pro-0.0.91/MANIFEST.in
--rw-rw-rw-   0        0        0     1280 2023-07-09 08:44:24.189172 irene_pro-0.0.91/PKG-INFO
--rw-rw-rw-   0        0        0      715 2023-06-30 07:10:26.000000 irene_pro-0.0.91/README.md
-drwxrwxrwx   0        0        0        0 2023-07-09 08:44:24.157246 irene_pro-0.0.91/irene_pro/
--rw-rw-rw-   0        0        0        0 2023-06-30 07:27:47.000000 irene_pro-0.0.91/irene_pro/__init__.py
--rw-rw-rw-   0        0        0     8188 2023-07-06 14:04:14.000000 irene_pro-0.0.91/irene_pro/logics.py
--rw-rw-rw-   0        0        0    36395 2023-07-09 08:42:18.000000 irene_pro-0.0.91/irene_pro/widgets.py
-drwxrwxrwx   0        0        0        0 2023-07-09 08:44:24.184384 irene_pro-0.0.91/irene_pro.egg-info/
--rw-rw-rw-   0        0        0     1280 2023-07-09 08:44:24.000000 irene_pro-0.0.91/irene_pro.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      265 2023-07-09 08:44:24.000000 irene_pro-0.0.91/irene_pro.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-09 08:44:24.000000 irene_pro-0.0.91/irene_pro.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2023-07-09 08:44:24.000000 irene_pro-0.0.91/irene_pro.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-09 08:44:24.000000 irene_pro-0.0.91/irene_pro.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-09 08:44:24.193175 irene_pro-0.0.91/setup.cfg
--rw-rw-rw-   0        0        0     1164 2023-07-09 08:42:33.000000 irene_pro-0.0.91/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-10 07:03:29.690910 irene_pro-0.0.92/
+-rw-rw-rw-   0        0        0      227 2023-06-30 07:10:26.000000 irene_pro-0.0.92/LICENSE
+-rw-rw-rw-   0        0        0       14 2023-06-30 07:10:26.000000 irene_pro-0.0.92/MANIFEST.in
+-rw-rw-rw-   0        0        0     1280 2023-07-10 07:03:29.689914 irene_pro-0.0.92/PKG-INFO
+-rw-rw-rw-   0        0        0      715 2023-06-30 07:10:26.000000 irene_pro-0.0.92/README.md
+drwxrwxrwx   0        0        0        0 2023-07-10 07:03:29.668970 irene_pro-0.0.92/irene_pro/
+-rw-rw-rw-   0        0        0        0 2023-06-30 07:27:47.000000 irene_pro-0.0.92/irene_pro/__init__.py
+-rw-rw-rw-   0        0        0     8188 2023-07-06 14:04:14.000000 irene_pro-0.0.92/irene_pro/logics.py
+-rw-rw-rw-   0        0        0    36096 2023-07-10 07:02:00.000000 irene_pro-0.0.92/irene_pro/widgets.py
+drwxrwxrwx   0        0        0        0 2023-07-10 07:03:29.686922 irene_pro-0.0.92/irene_pro.egg-info/
+-rw-rw-rw-   0        0        0     1280 2023-07-10 07:03:29.000000 irene_pro-0.0.92/irene_pro.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      265 2023-07-10 07:03:29.000000 irene_pro-0.0.92/irene_pro.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-10 07:03:29.000000 irene_pro-0.0.92/irene_pro.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2023-07-10 07:03:29.000000 irene_pro-0.0.92/irene_pro.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-10 07:03:29.000000 irene_pro-0.0.92/irene_pro.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-10 07:03:29.691910 irene_pro-0.0.92/setup.cfg
+-rw-rw-rw-   0        0        0     1164 2023-07-10 07:02:07.000000 irene_pro-0.0.92/setup.py
```

### Comparing `irene_pro-0.0.91/PKG-INFO` & `irene_pro-0.0.92/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irene_pro
-Version: 0.0.91
+Version: 0.0.92
 Summary: Use customized GUI
 Author: Irene coldsober
 Author-email: <irene.study.2023@gmail.com>
 Keywords: tkinter,widget,gui
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `irene_pro-0.0.91/README.md` & `irene_pro-0.0.92/README.md`

 * *Files identical despite different names*

### Comparing `irene_pro-0.0.91/irene_pro/logics.py` & `irene_pro-0.0.92/irene_pro/logics.py`

 * *Files identical despite different names*

### Comparing `irene_pro-0.0.91/irene_pro/widgets.py` & `irene_pro-0.0.92/irene_pro/widgets.py`

 * *Files 7% similar despite different names*

```diff
@@ -116,15 +116,14 @@
 
     def insert_data(self,data, wrap_length = 70, odd_color = 'gray70', even_color = 'khaki'):
         self.alter_rows(odd_color=odd_color, even_color=even_color)
         def wrapping(data_list):
             """I assume that datalist is a list as the name implies"""
             all_row = []
             for item in data_list:
-                # print(f"CURRENT ITEM: {item}")
                 if type(item) == str:
                     wrapped = wrap(item, wrap_length)
                     all_row.append("\n".join(wrapped))
                 else:
                     all_row.append(item)
                 
             return all_row
@@ -133,34 +132,30 @@
             if type(data[0]) not in [list, tuple]:
                 if self.include_index:
                     tag = ('odd')
                 
                     if self.index_for_single_list_data % 2 ==0:
                         tag = ('even',)
                     data_wrapped = wrapping(data)
-                    print(" [K: ] {data_wrapped}")
                     self.insert("", index=self.index_for_single_list_data,text=self.index_for_single_list_data + 1, values = data_wrapped, tags = tag)
                 else:
                     data_wrapped = wrapping(data)
-                    print(" [I: ] {data_wrapped}")
                     self.insert("", index=self.index_for_single_list_data, values = data_wrapped)
                 self.index_for_single_list_data += 1
                 
             else:
                 for index, row in enumerate(data):
                     tag = ('odd')
                     if self.index_for_single_list_data % 2 ==0:
                         tag = ('even',)
                     if self.include_index:
                         data_wrapped = wrapping(row)
-                        print(" [H: ] {data_wrapped}")
                         self.insert("", index=index,text=self.index_for_single_list_data+1, values = data_wrapped, tags=tag)
                     else:
                         data_wrapped = wrapping(row)
-                        print(" [G: ] {data_wrapped}")
                         self.insert("", index=index, values = data_wrapped)
                     self.index_for_single_list_data += 1
         except IndexError:
             pass
 
 class btn(Button):
     def __init__(self, master,image = None, **kwargs):
@@ -416,20 +411,17 @@
             pass
         
         def remove_default():
             if self.get() == default:
                 self.set('')
         
         def set_default():
-            print("LEAVING COMBOBOX.....")
             if self.get().strip() == "" or len(self.get().strip()) == 0:
                 self.set(default)
-                print("[DEFAULT SET]")
-            else:
-                print(f"COMBO VALUE FOUND: {self.get().strip()}: length: {len(self.get().strip())}")
+            
 
         if self.cget('state') != 'readonly':
             if default:
                 self.set(default)
                 self.bind("<Button-1>", lambda e: remove_default())
                 self.bind("<Leave>", lambda e: set_default())
 
@@ -520,20 +512,22 @@
     
 
 class spinbox(ttk.Spinbox):
     def __init__(self, master, **kwargs):
         super().__init__(master =master, **kwargs)
 
 class calendar(Calendar):
-    def __init__(self, master, global_date_holder:Variable, date_holder_widget = None, create_toplevel = False, **kw):
+    def __init__(self, master, global_date_holder:Variable, date_holder_widget = None, create_toplevel = False, 
+                 destroy_after_set = True, **kw):
         super().__init__(master = master, **kw)
         self.master = master
         self.global_time_holder = global_date_holder
         self.datetime_fr = None
         self.choosen_date = date_holder_widget
+        self.destroy_after_set = destroy_after_set
         if not create_toplevel:
             self.datetime_fr = lframe(self.master)
             self.datetime_fr.pack(side=RIGHT, padx = w(2))
         else:
             # CREATE TOPLEVEL WINDOW TO HOLD THE CALENDAR AND THE TIME SELECTOR
             self.datetime_fr = Toplevel()
             self.datetime_fr.title("Select time and date")
@@ -599,15 +593,16 @@
                     self.choosen_date.insert(END, final_datetime)
                 except Exception:
                     try:
                         self.choosen_date.delete(0.0, END)
                         self.choosen_date.insert(END, final_datetime)
                     except Exception:
                         pass
-            self.datetime_fr.destroy()
+            if self.destroy_after_set:
+                self.datetime_fr.destroy()
             
             
         set_date = btn(master=self.datetime_fr3, text = "set date", command = set_selected)
         set_date.pack(side=LEFT, fill=X, expand=True)
         close = btn(master=self.datetime_fr3, text = "close", 
                          command = lambda: self.datetime_fr.destroy())
         close.pack(side=LEFT, fill=X, expand = True)
@@ -857,16 +852,16 @@
         details.pack(side = TOP, padx = w(1), pady = h(0), fill=X, expand = True, anchor = NW)
 
         close_btn = btn(fr, text = "close",activebackground = fr.cget('bg'), command = lambda: fr.destroy())
         close_btn.pack(side = TOP, padx = w(1), pady = h(0), fill=X, expand = True, anchor = NW)
 
         return delete_btn, edit_btn, status, details
 
-def get_parent(widget):
+def get_parent(widget, root_of_app):
     parent_name = widget.winfo_parent()
-    parent_widget = Widget._nametowidget(parent_name)
+    parent_widget = root_of_app.nametowidget(parent_name)
     return parent_widget
 
 # CONSTANTS
 comb_syle = 'comb.TCombobox'
 check_style = "TCheckbutton"
 radio_style = "Custom.TRadiobutton"
```

### Comparing `irene_pro-0.0.91/irene_pro.egg-info/PKG-INFO` & `irene_pro-0.0.92/irene_pro.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irene-pro
-Version: 0.0.91
+Version: 0.0.92
 Summary: Use customized GUI
 Author: Irene coldsober
 Author-email: <irene.study.2023@gmail.com>
 Keywords: tkinter,widget,gui
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `irene_pro-0.0.91/setup.py` & `irene_pro-0.0.92/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 00000090: 286f 732e 7061 7468 2e6a 6f69 6e28 6865  (os.path.join(he
 000000a0: 7265 2c20 2252 4541 444d 452e 6d64 2229  re, "README.md")
 000000b0: 2c20 656e 636f 6469 6e67 3d22 7574 662d  , encoding="utf-
 000000c0: 3822 2920 6173 2066 683a 0d0a 2020 2020  8") as fh:..    
 000000d0: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
 000000e0: 203d 2022 5c6e 2220 2b20 6668 2e72 6561   = "\n" + fh.rea
 000000f0: 6428 290d 0a0d 0a56 4552 5349 4f4e 203d  d()....VERSION =
-00000100: 2027 302e 302e 3931 270d 0a44 4553 4352   '0.0.91'..DESCR
+00000100: 2027 302e 302e 3932 270d 0a44 4553 4352   '0.0.92'..DESCR
 00000110: 4950 5449 4f4e 203d 2027 5573 6520 6375  IPTION = 'Use cu
 00000120: 7374 6f6d 697a 6564 2047 5549 270d 0a4c  stomized GUI'..L
 00000130: 4f4e 475f 4445 5343 5249 5054 494f 4e20  ONG_DESCRIPTION 
 00000140: 3d20 2741 2070 6163 6b61 6765 2074 6861  = 'A package tha
 00000150: 7420 616c 6c6f 7773 2079 6f75 2074 6f20  t allows you to 
 00000160: 7573 6520 7374 796c 6573 2061 6e64 2077  use styles and w
 00000170: 6964 6765 7420 6f66 2073 7570 6572 206c  idget of super l
```

