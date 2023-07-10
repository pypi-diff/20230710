# Comparing `tmp/irene_pro-0.0.92.tar.gz` & `tmp/irene_pro-0.0.93.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "irene_pro-0.0.92.tar", last modified: Mon Jul 10 07:03:29 2023, max compression
+gzip compressed data, was "irene_pro-0.0.93.tar", last modified: Mon Jul 10 09:13:19 2023, max compression
```

## Comparing `irene_pro-0.0.92.tar` & `irene_pro-0.0.93.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-07-10 07:03:29.690910 irene_pro-0.0.92/
--rw-rw-rw-   0        0        0      227 2023-06-30 07:10:26.000000 irene_pro-0.0.92/LICENSE
--rw-rw-rw-   0        0        0       14 2023-06-30 07:10:26.000000 irene_pro-0.0.92/MANIFEST.in
--rw-rw-rw-   0        0        0     1280 2023-07-10 07:03:29.689914 irene_pro-0.0.92/PKG-INFO
--rw-rw-rw-   0        0        0      715 2023-06-30 07:10:26.000000 irene_pro-0.0.92/README.md
-drwxrwxrwx   0        0        0        0 2023-07-10 07:03:29.668970 irene_pro-0.0.92/irene_pro/
--rw-rw-rw-   0        0        0        0 2023-06-30 07:27:47.000000 irene_pro-0.0.92/irene_pro/__init__.py
--rw-rw-rw-   0        0        0     8188 2023-07-06 14:04:14.000000 irene_pro-0.0.92/irene_pro/logics.py
--rw-rw-rw-   0        0        0    36096 2023-07-10 07:02:00.000000 irene_pro-0.0.92/irene_pro/widgets.py
-drwxrwxrwx   0        0        0        0 2023-07-10 07:03:29.686922 irene_pro-0.0.92/irene_pro.egg-info/
--rw-rw-rw-   0        0        0     1280 2023-07-10 07:03:29.000000 irene_pro-0.0.92/irene_pro.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      265 2023-07-10 07:03:29.000000 irene_pro-0.0.92/irene_pro.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-10 07:03:29.000000 irene_pro-0.0.92/irene_pro.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2023-07-10 07:03:29.000000 irene_pro-0.0.92/irene_pro.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-10 07:03:29.000000 irene_pro-0.0.92/irene_pro.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-10 07:03:29.691910 irene_pro-0.0.92/setup.cfg
--rw-rw-rw-   0        0        0     1164 2023-07-10 07:02:07.000000 irene_pro-0.0.92/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-10 09:13:19.168541 irene_pro-0.0.93/
+-rw-rw-rw-   0        0        0      227 2023-06-30 07:10:26.000000 irene_pro-0.0.93/LICENSE
+-rw-rw-rw-   0        0        0       14 2023-06-30 07:10:26.000000 irene_pro-0.0.93/MANIFEST.in
+-rw-rw-rw-   0        0        0     1280 2023-07-10 09:13:19.166548 irene_pro-0.0.93/PKG-INFO
+-rw-rw-rw-   0        0        0      715 2023-06-30 07:10:26.000000 irene_pro-0.0.93/README.md
+drwxrwxrwx   0        0        0        0 2023-07-10 09:13:19.146599 irene_pro-0.0.93/irene_pro/
+-rw-rw-rw-   0        0        0        0 2023-06-30 07:27:47.000000 irene_pro-0.0.93/irene_pro/__init__.py
+-rw-rw-rw-   0        0        0     8188 2023-07-06 14:04:14.000000 irene_pro-0.0.93/irene_pro/logics.py
+-rw-rw-rw-   0        0        0    36215 2023-07-10 09:11:14.000000 irene_pro-0.0.93/irene_pro/widgets.py
+drwxrwxrwx   0        0        0        0 2023-07-10 09:13:19.162557 irene_pro-0.0.93/irene_pro.egg-info/
+-rw-rw-rw-   0        0        0     1280 2023-07-10 09:13:19.000000 irene_pro-0.0.93/irene_pro.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      265 2023-07-10 09:13:19.000000 irene_pro-0.0.93/irene_pro.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-10 09:13:19.000000 irene_pro-0.0.93/irene_pro.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2023-07-10 09:13:19.000000 irene_pro-0.0.93/irene_pro.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-10 09:13:19.000000 irene_pro-0.0.93/irene_pro.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-10 09:13:19.169538 irene_pro-0.0.93/setup.cfg
+-rw-rw-rw-   0        0        0     1164 2023-07-10 09:11:37.000000 irene_pro-0.0.93/setup.py
```

### Comparing `irene_pro-0.0.92/PKG-INFO` & `irene_pro-0.0.93/irene_pro.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: irene_pro
-Version: 0.0.92
+Name: irene-pro
+Version: 0.0.93
 Summary: Use customized GUI
 Author: Irene coldsober
 Author-email: <irene.study.2023@gmail.com>
 Keywords: tkinter,widget,gui
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `irene_pro-0.0.92/README.md` & `irene_pro-0.0.93/README.md`

 * *Files identical despite different names*

### Comparing `irene_pro-0.0.92/irene_pro/logics.py` & `irene_pro-0.0.93/irene_pro/logics.py`

 * *Files identical despite different names*

### Comparing `irene_pro-0.0.92/irene_pro/widgets.py` & `irene_pro-0.0.93/irene_pro/widgets.py`

 * *Files 1% similar despite different names*

```diff
@@ -248,32 +248,32 @@
 class panedw(ttk.Panedwindow):
     def __init__(self, master, **kwargs):
         super().__init__(master=master, **kwargs)
 
 class EntryBtns:
     def __init__(self, parent, saved_data_holder, entry_tags, entry_fr_height = h(50),
                         entry_fr_side = TOP, fill = X, widget_2_create = 'entry'
-                        , browse = False, ent_id_width = 5, default = None):
+                        , browse = False, ent_id_width = 5, default = None, keep_default = False):
         
         self.saved_data_holder = saved_data_holder
         self.entry_tags = entry_tags
         self.entry_fr_height = entry_fr_height
         self.entry_fr_side = entry_fr_side
         self.widget_2_create = widget_2_create
         self.default = default
 
         self.fr = frame(master = parent)
         self.fr.pack(side=entry_fr_side, fill=fill, padx = w(2), expand = True)
         
         if widget_2_create == 'entry':
-            self.ent = entry(self.fr, fg="gray50", default=default)
+            self.ent = entry(self.fr, fg="gray50", default=default, keep_default=keep_default)
             self.ent.pack(side=LEFT, fill=X, ipadx=w(40), expand = True, pady = h(2))
 
         elif widget_2_create == 'text':
-            self.ent = Textb(self.fr, default=default, height = h(4))
+            self.ent = Textb(self.fr, default=default, height = h(4), keep_default=keep_default)
             self.ent.pack(padx = w(1), pady=h(1), side = LEFT, expand = True, fill = X)
                 
 
         self.ent_id = entry(self.fr, width = ent_id_width)
         self.ent_id.pack(side=LEFT, padx = w(2), pady = h(2))
         
         # AVOID EDITING ENT_ID
@@ -359,18 +359,18 @@
     if color[1] is not None:
         if color_holder:
             color_holder.delete(0, END)
             color_holder.insert(END, color[1])
 
 #==============ENTRY===============
 class entry(Entry):
-    def __init__(self, master, default = None, font = ('arial', w(12)), **kwargs):
+    def __init__(self, master, default = None, keep_default = False, font = ('arial', w(12)), **kwargs):
         super().__init__(master = master, bg = master['bg'], highlightbackground='gray50', highlightcolor="gray50", highlightthickness=1,bd=0, font = font, **kwargs)
         
-        if default:
+        if default and not keep_default:
             self.bind("<KeyPress>", lambda e: remove_txt())
             self.bind("<Leave>", lambda e: add_txt())
             self.delete(0, END)
             self.insert(END, default)
             self.config(fg = "gray50")
 
         num = re.compile("\d{1,}")
```

### Comparing `irene_pro-0.0.92/irene_pro.egg-info/PKG-INFO` & `irene_pro-0.0.93/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: irene-pro
-Version: 0.0.92
+Name: irene_pro
+Version: 0.0.93
 Summary: Use customized GUI
 Author: Irene coldsober
 Author-email: <irene.study.2023@gmail.com>
 Keywords: tkinter,widget,gui
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `irene_pro-0.0.92/setup.py` & `irene_pro-0.0.93/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 00000090: 286f 732e 7061 7468 2e6a 6f69 6e28 6865  (os.path.join(he
 000000a0: 7265 2c20 2252 4541 444d 452e 6d64 2229  re, "README.md")
 000000b0: 2c20 656e 636f 6469 6e67 3d22 7574 662d  , encoding="utf-
 000000c0: 3822 2920 6173 2066 683a 0d0a 2020 2020  8") as fh:..    
 000000d0: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
 000000e0: 203d 2022 5c6e 2220 2b20 6668 2e72 6561   = "\n" + fh.rea
 000000f0: 6428 290d 0a0d 0a56 4552 5349 4f4e 203d  d()....VERSION =
-00000100: 2027 302e 302e 3932 270d 0a44 4553 4352   '0.0.92'..DESCR
+00000100: 2027 302e 302e 3933 270d 0a44 4553 4352   '0.0.93'..DESCR
 00000110: 4950 5449 4f4e 203d 2027 5573 6520 6375  IPTION = 'Use cu
 00000120: 7374 6f6d 697a 6564 2047 5549 270d 0a4c  stomized GUI'..L
 00000130: 4f4e 475f 4445 5343 5249 5054 494f 4e20  ONG_DESCRIPTION 
 00000140: 3d20 2741 2070 6163 6b61 6765 2074 6861  = 'A package tha
 00000150: 7420 616c 6c6f 7773 2079 6f75 2074 6f20  t allows you to 
 00000160: 7573 6520 7374 796c 6573 2061 6e64 2077  use styles and w
 00000170: 6964 6765 7420 6f66 2073 7570 6572 206c  idget of super l
```

