# Comparing `tmp/BaseDT-0.1.0.tar.gz` & `tmp/BaseDT-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/BaseDT-0.1.0.tar", last modified: Wed Jun 21 03:39:22 2023, max compression
+gzip compressed data, was "dist/BaseDT-0.1.1.tar", last modified: Mon Jun 26 06:08:23 2023, max compression
```

## Comparing `BaseDT-0.1.0.tar` & `BaseDT-0.1.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-06-21 03:39:22.000000 BaseDT-0.1.0/
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-06-21 03:39:22.000000 BaseDT-0.1.0/BaseDT/
--rw-rw-r--   0 user      (1001) user      (1001)       32 2023-06-21 03:34:40.000000 BaseDT-0.1.0/BaseDT/__init__.py
--rw-rw-r--   0 user      (1001) user      (1001)    35422 2023-06-19 05:49:30.000000 BaseDT-0.1.0/BaseDT/data.py
--rw-rw-r--   0 user      (1001) user      (1001)    12037 2023-06-19 05:43:54.000000 BaseDT-0.1.0/BaseDT/data_image.py
--rw-rw-r--   0 user      (1001) user      (1001)    37236 2023-06-09 06:59:00.000000 BaseDT-0.1.0/BaseDT/dataset.py
--rw-rw-r--   0 user      (1001) user      (1001)     1020 2023-06-19 05:43:54.000000 BaseDT-0.1.0/BaseDT/io.py
--rw-rw-r--   0 user      (1001) user      (1001)    15667 2023-06-21 03:33:07.000000 BaseDT-0.1.0/BaseDT/plot.py
--rw-rw-r--   0 user      (1001) user      (1001)    18654 2023-06-19 05:47:08.000000 BaseDT-0.1.0/BaseDT/utils.py
--rw-rw-r--   0 user      (1001) user      (1001)     1224 2023-06-21 03:31:23.000000 BaseDT-0.1.0/BaseDT/version.py
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-06-21 03:39:22.000000 BaseDT-0.1.0/BaseDT.egg-info/
--rw-rw-r--   0 user      (1001) user      (1001)      314 2023-06-21 03:39:22.000000 BaseDT-0.1.0/BaseDT.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1001) user      (1001)      383 2023-06-21 03:39:22.000000 BaseDT-0.1.0/BaseDT.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1001) user      (1001)        1 2023-06-21 03:39:22.000000 BaseDT-0.1.0/BaseDT.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1001) user      (1001)       49 2023-06-21 03:39:22.000000 BaseDT-0.1.0/BaseDT.egg-info/entry_points.txt
--rw-rw-r--   0 user      (1001) user      (1001)       43 2023-06-21 03:39:22.000000 BaseDT-0.1.0/BaseDT.egg-info/requires.txt
--rw-rw-r--   0 user      (1001) user      (1001)        7 2023-06-21 03:39:22.000000 BaseDT-0.1.0/BaseDT.egg-info/top_level.txt
--rw-rw-r--   0 user      (1001) user      (1001)        1 2023-02-02 07:26:47.000000 BaseDT-0.1.0/BaseDT.egg-info/zip-safe
--rw-rw-r--   0 user      (1001) user      (1001)       40 2023-04-06 03:45:54.000000 BaseDT-0.1.0/MANIFEST.in
--rw-rw-r--   0 user      (1001) user      (1001)      314 2023-06-21 03:39:22.000000 BaseDT-0.1.0/PKG-INFO
--rw-rw-r--   0 user      (1001) user      (1001)       42 2023-05-31 10:06:54.000000 BaseDT-0.1.0/install_requires.txt
--rw-rw-r--   0 user      (1001) user      (1001)       38 2023-06-21 03:39:22.000000 BaseDT-0.1.0/setup.cfg
--rw-rw-r--   0 user      (1001) user      (1001)     4245 2023-06-21 03:39:15.000000 BaseDT-0.1.0/setup.py
+drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-06-26 06:08:23.000000 BaseDT-0.1.1/
+drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-06-26 06:08:23.000000 BaseDT-0.1.1/BaseDT/
+-rw-rw-r--   0 user      (1001) user      (1001)       32 2023-06-21 03:34:40.000000 BaseDT-0.1.1/BaseDT/__init__.py
+-rw-rw-r--   0 user      (1001) user      (1001)    35592 2023-06-26 03:44:16.000000 BaseDT-0.1.1/BaseDT/data.py
+-rw-rw-r--   0 user      (1001) user      (1001)    12037 2023-06-19 05:43:54.000000 BaseDT-0.1.1/BaseDT/data_image.py
+-rw-rw-r--   0 user      (1001) user      (1001)    37314 2023-06-26 06:07:55.000000 BaseDT-0.1.1/BaseDT/dataset.py
+-rw-rw-r--   0 user      (1001) user      (1001)     1020 2023-06-19 05:43:54.000000 BaseDT-0.1.1/BaseDT/io.py
+-rw-rw-r--   0 user      (1001) user      (1001)    15668 2023-06-26 05:44:24.000000 BaseDT-0.1.1/BaseDT/plot.py
+-rw-rw-r--   0 user      (1001) user      (1001)    18654 2023-06-19 05:47:08.000000 BaseDT-0.1.1/BaseDT/utils.py
+-rw-rw-r--   0 user      (1001) user      (1001)     1217 2023-06-26 03:45:13.000000 BaseDT-0.1.1/BaseDT/version.py
+drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-06-26 06:08:23.000000 BaseDT-0.1.1/BaseDT.egg-info/
+-rw-rw-r--   0 user      (1001) user      (1001)      314 2023-06-26 06:08:23.000000 BaseDT-0.1.1/BaseDT.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1001) user      (1001)      383 2023-06-26 06:08:23.000000 BaseDT-0.1.1/BaseDT.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1001) user      (1001)        1 2023-06-26 06:08:23.000000 BaseDT-0.1.1/BaseDT.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1001) user      (1001)       49 2023-06-26 06:08:23.000000 BaseDT-0.1.1/BaseDT.egg-info/entry_points.txt
+-rw-rw-r--   0 user      (1001) user      (1001)       43 2023-06-26 06:08:23.000000 BaseDT-0.1.1/BaseDT.egg-info/requires.txt
+-rw-rw-r--   0 user      (1001) user      (1001)        7 2023-06-26 06:08:23.000000 BaseDT-0.1.1/BaseDT.egg-info/top_level.txt
+-rw-rw-r--   0 user      (1001) user      (1001)        1 2023-02-02 07:26:47.000000 BaseDT-0.1.1/BaseDT.egg-info/zip-safe
+-rw-rw-r--   0 user      (1001) user      (1001)       40 2023-04-06 03:45:54.000000 BaseDT-0.1.1/MANIFEST.in
+-rw-rw-r--   0 user      (1001) user      (1001)      314 2023-06-26 06:08:23.000000 BaseDT-0.1.1/PKG-INFO
+-rw-rw-r--   0 user      (1001) user      (1001)       42 2023-05-31 10:06:54.000000 BaseDT-0.1.1/install_requires.txt
+-rw-rw-r--   0 user      (1001) user      (1001)       38 2023-06-26 06:08:23.000000 BaseDT-0.1.1/setup.cfg
+-rw-rw-r--   0 user      (1001) user      (1001)     4245 2023-06-26 03:45:05.000000 BaseDT-0.1.1/setup.py
```

### Comparing `BaseDT-0.1.0/BaseDT/data.py` & `BaseDT-0.1.1/BaseDT/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,28 +69,30 @@
         if type(self.data_source) == np.ndarray:
             self.value = self.data_source
         else:
             # TODO 检查合法性
             pass
         self.value = self.value.astype(self.get_attribute("data_type"))
         self.raw_value = self.value
+        self.init_by_backbone = False
         self.fig_save = None
         self.fig_save_cfg = None
         self.fig_show_cfg = None
         self.fig_save_canvas = None
         self.fig_save = None
         self.ax_save = None
         self.dpi = None
         self.width = None
         self.height = None
         self._image = None
 
         if self.get_attribute("backbone"):
             # for key, value in self._backbone_args[self.get_attribute("backbone")].items():
             #     print(key,value)
+            self.init_by_backbone = True
             self.value = ImageData(data_source, **self._backbone_args[self.get_attribute("backbone")]).value
             self.__dict__.update(self._backbone_args[self.get_attribute("backbone")])#更新私有变量列表
         else:
             if self.get_attribute("to_rgb") == False and len(self.value.shape)>=3:
                 self._rgb2gray()
             elif self.get_attribute("to_rgb") == True:
                 self._to3channel()
@@ -123,15 +125,18 @@
                   fig_show_cfg=dict(frameon=False)):
         self.fig_save = None
         self.fig_save_cfg = fig_save_cfg
         self.fig_show_cfg = fig_show_cfg
         (self.fig_save_canvas, self.fig_save,
          self.ax_save) = self._initialize_fig(fig_save_cfg)
         self.dpi = self.fig_save.get_dpi()
-        image_rgb = cv2.cvtColor(self.raw_value, cv2.COLOR_BGR2RGB)
+        if self.init_by_backbone:
+            image_rgb = cv2.cvtColor(self.raw_value, cv2.COLOR_BGR2RGB)
+        else:
+            image_rgb = self.raw_value
         self._set_image(image_rgb)
 
     #保护方法，不给用户调用
     def _rgb2gray(self):
         gray = np.dot(self.value, [0.2989, 0.5870, 0.1140])
         gray = np.clip(gray, 0, 255).astype(np.uint8)
         self.value = gray
```

### Comparing `BaseDT-0.1.0/BaseDT/data_image.py` & `BaseDT-0.1.1/BaseDT/data_image.py`

 * *Files identical despite different names*

### Comparing `BaseDT-0.1.0/BaseDT/dataset.py` & `BaseDT-0.1.1/BaseDT/dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -802,14 +802,16 @@
     # # 保存为 CSV 文件
     file_name = data_path.rsplit(".",1)
     train_file = file_name[0]+"_train."+file_name[1]
     val_file = file_name[0]+"_val."+file_name[1]
     np.savetxt(train_file, train_data_with_header, delimiter=",", fmt="%s")
     np.savetxt(val_file, val_data_with_header, delimiter=",", fmt="%s")
     print("训练集保存至{}，验证集保存至{}。".format(train_file, val_file))
+    if normalize == True:
+        return train_x,train_y, val_x, val_y,scaler
     return train_x,train_y, val_x, val_y
 
 def split_tab_dataset_class(data_path, data_column,label_column=[-1],train_val_ratio=0.8,random_seed=42):
     # 读取提取后的特征和标签
     data = np.loadtxt(data_path, dtype=float, delimiter=',',skiprows=1,usecols=data_column)
     label =  np.loadtxt(data_path, dtype=float, delimiter=',',skiprows=1,usecols=label_column)
     # 获得所有标签
```

### Comparing `BaseDT-0.1.0/BaseDT/io.py` & `BaseDT-0.1.1/BaseDT/io.py`

 * *Files identical despite different names*

### Comparing `BaseDT-0.1.0/BaseDT/plot.py` & `BaseDT-0.1.1/BaseDT/plot.py`

 * *Files 1% similar despite different names*

```diff
@@ -247,15 +247,15 @@
     texts = []
     max_length = 12 # 文本长度限制
     if '标签' in result:
         texts.append('Pred_label: {}'.format(result['标签']))
     if '置信度' in result:
         texts.append('Pred_score: {:.2f}'.format(result['置信度']))
     if '预测结果' in result:
-        texts.append('Pred_label: {}'.format(result['预测结果'][:max_length]))
+        texts.append('Pred_result: {}'.format(result['预测结果'][:max_length]))
     text = '\n'.join(texts)
     #fig = plt.figure()
     image.init_plt()
     img_tmp = image._image
     img_scale = get_adaptive_scale(img_tmp.shape[:2])
     DEFAULT_TEXT_CFG['size'] = int(img_scale * 5)
     pos = np.array([[img_scale*5, img_scale*5]], dtype=int)
```

### Comparing `BaseDT-0.1.0/BaseDT/utils.py` & `BaseDT-0.1.1/BaseDT/utils.py`

 * *Files identical despite different names*

### Comparing `BaseDT-0.1.0/BaseDT/version.py` & `BaseDT-0.1.1/BaseDT/version.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os
 
-__version__='0.1.0'
+__version__='0.1.1'
 __path__=os.path.abspath(os.getcwd())
 
 def parse_version_info(version_str):
     version_info = []
     for x in version_str.split('.'):
         if x.isdigit():
             version_info.append(int(x))
@@ -17,16 +17,15 @@
 def hello():
                                                  
     print("""
     ____                  ____  ______
    / __ )____ _________  / __ \/_  __/
   / __  / __ `/ ___/ _ \/ / / / / /   
  / /_/ / /_/ (__  )  __/ /_/ / / /    
-/_____/\__,_/____/\___/_____/ /_/     
-                                                                           
+/_____/\__,_/____/\___/_____/ /_/                                                                          
     """)
     print("BaseDT 是一个功能强大且易于扩展的数据处理工具。")
     print("BaseDT is a powerful and easily extensible data processing tool.")
     print("相关网址：")
     print("-文档网址 :  https://xedu.readthedocs.io")
     print("-官网网址 :  https://www.openinnolab.org.cn/pjEdu/xedu/baseedu")
```

### Comparing `BaseDT-0.1.0/setup.py` & `BaseDT-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,15 +75,15 @@
                 yield item
 
     packages = list(gen_packages_items())
     return packages
 
 setup(
     name='BaseDT',
-    version='0.1.0',
+    version='0.1.1',
     # version='0.0.1rc1',
     description='BaseDT is a data-processing  tool including data, dataset, io and plot.',
     license='MIT License',
     author='OpenXLab',
     author_email='wangbolun@pjlab.org.cn',
     url='https://github.com/OpenXLab-Edu/OpenMMLab-Edu',
     packages=find_packages(),
```

