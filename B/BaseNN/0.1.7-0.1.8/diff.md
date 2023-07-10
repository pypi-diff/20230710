# Comparing `tmp/BaseNN-0.1.7.tar.gz` & `tmp/BaseNN-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/BaseNN-0.1.7.tar", last modified: Thu Jul  6 06:51:23 2023, max compression
+gzip compressed data, was "dist/BaseNN-0.1.8.tar", last modified: Mon Jul 10 08:35:04 2023, max compression
```

## Comparing `BaseNN-0.1.7.tar` & `BaseNN-0.1.8.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-07-06 06:51:23.000000 BaseNN-0.1.7/
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-07-06 06:51:23.000000 BaseNN-0.1.7/BaseNN/
--rw-rw-r--   0 user      (1001) user      (1001)    39047 2023-07-06 06:50:46.000000 BaseNN-0.1.7/BaseNN/BaseNN.py
--rw-rw-r--   0 user      (1001) user      (1001)      270 2023-05-24 09:07:14.000000 BaseNN-0.1.7/BaseNN/__init__.py
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-07-06 06:51:23.000000 BaseNN-0.1.7/BaseNN/examples/
--rw-rw-r--   0 user      (1001) user      (1001)    24607 2023-07-06 06:49:25.000000 BaseNN-0.1.7/BaseNN/examples/BaseNN_demo.py
--rw-rw-r--   0 user      (1001) user      (1001)        0 2022-08-26 07:13:38.000000 BaseNN-0.1.7/BaseNN/examples/__init__.py
--rw-rw-r--   0 user      (1001) user      (1001)     3059 2023-04-13 07:47:30.000000 BaseNN-0.1.7/BaseNN/examples/pkl2pth.py
--rw-r--r--   0 user      (1001) user      (1001)     4409 2023-05-22 08:15:12.000000 BaseNN-0.1.7/BaseNN/load_data.py
--rw-rw-r--   0 user      (1001) user      (1001)     1256 2023-07-06 06:29:56.000000 BaseNN-0.1.7/BaseNN/version.py
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-07-06 06:51:23.000000 BaseNN-0.1.7/BaseNN.egg-info/
--rw-rw-r--   0 user      (1001) user      (1001)      346 2023-07-06 06:51:23.000000 BaseNN-0.1.7/BaseNN.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1001) user      (1001)      375 2023-07-06 06:51:23.000000 BaseNN-0.1.7/BaseNN.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1001) user      (1001)        1 2023-07-06 06:51:23.000000 BaseNN-0.1.7/BaseNN.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1001) user      (1001)       49 2023-07-06 06:51:23.000000 BaseNN-0.1.7/BaseNN.egg-info/entry_points.txt
--rw-rw-r--   0 user      (1001) user      (1001)       80 2023-07-06 06:51:23.000000 BaseNN-0.1.7/BaseNN.egg-info/requires.txt
--rw-rw-r--   0 user      (1001) user      (1001)        7 2023-07-06 06:51:23.000000 BaseNN-0.1.7/BaseNN.egg-info/top_level.txt
--rw-rw-r--   0 user      (1001) user      (1001)        1 2022-11-18 03:21:26.000000 BaseNN-0.1.7/BaseNN.egg-info/zip-safe
--rw-rw-r--   0 user      (1001) user      (1001)      346 2023-07-06 06:51:23.000000 BaseNN-0.1.7/PKG-INFO
--rw-rw-r--   0 user      (1001) user      (1001)       38 2023-07-06 06:51:23.000000 BaseNN-0.1.7/setup.cfg
--rw-rw-r--   0 user      (1001) user      (1001)     3827 2023-07-06 06:29:37.000000 BaseNN-0.1.7/setup.py
+drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-07-10 08:35:04.000000 BaseNN-0.1.8/
+drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-07-10 08:35:04.000000 BaseNN-0.1.8/BaseNN/
+-rw-rw-r--   0 user      (1001) user      (1001)    39033 2023-07-07 06:54:05.000000 BaseNN-0.1.8/BaseNN/BaseNN.py
+-rw-rw-r--   0 user      (1001) user      (1001)      270 2023-05-24 09:07:14.000000 BaseNN-0.1.8/BaseNN/__init__.py
+drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-07-10 08:35:04.000000 BaseNN-0.1.8/BaseNN/examples/
+-rw-rw-r--   0 user      (1001) user      (1001)    26768 2023-07-10 08:29:41.000000 BaseNN-0.1.8/BaseNN/examples/BaseNN_demo.py
+-rw-rw-r--   0 user      (1001) user      (1001)        0 2022-08-26 07:13:38.000000 BaseNN-0.1.8/BaseNN/examples/__init__.py
+-rw-rw-r--   0 user      (1001) user      (1001)     3059 2023-04-13 07:47:30.000000 BaseNN-0.1.8/BaseNN/examples/pkl2pth.py
+-rw-r--r--   0 user      (1001) user      (1001)     4409 2023-05-22 08:15:12.000000 BaseNN-0.1.8/BaseNN/load_data.py
+-rw-rw-r--   0 user      (1001) user      (1001)     1256 2023-07-07 06:54:47.000000 BaseNN-0.1.8/BaseNN/version.py
+drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-07-10 08:35:04.000000 BaseNN-0.1.8/BaseNN.egg-info/
+-rw-rw-r--   0 user      (1001) user      (1001)      346 2023-07-10 08:35:04.000000 BaseNN-0.1.8/BaseNN.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1001) user      (1001)      375 2023-07-10 08:35:04.000000 BaseNN-0.1.8/BaseNN.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1001) user      (1001)        1 2023-07-10 08:35:04.000000 BaseNN-0.1.8/BaseNN.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1001) user      (1001)       49 2023-07-10 08:35:04.000000 BaseNN-0.1.8/BaseNN.egg-info/entry_points.txt
+-rw-rw-r--   0 user      (1001) user      (1001)       80 2023-07-10 08:35:04.000000 BaseNN-0.1.8/BaseNN.egg-info/requires.txt
+-rw-rw-r--   0 user      (1001) user      (1001)        7 2023-07-10 08:35:04.000000 BaseNN-0.1.8/BaseNN.egg-info/top_level.txt
+-rw-rw-r--   0 user      (1001) user      (1001)        1 2022-11-18 03:21:26.000000 BaseNN-0.1.8/BaseNN.egg-info/zip-safe
+-rw-rw-r--   0 user      (1001) user      (1001)      346 2023-07-10 08:35:04.000000 BaseNN-0.1.8/PKG-INFO
+-rw-rw-r--   0 user      (1001) user      (1001)       38 2023-07-10 08:35:04.000000 BaseNN-0.1.8/setup.cfg
+-rw-rw-r--   0 user      (1001) user      (1001)     3827 2023-07-07 06:54:38.000000 BaseNN-0.1.8/setup.py
```

### Comparing `BaseNN-0.1.7/BaseNN/BaseNN.py` & `BaseNN-0.1.8/BaseNN/BaseNN.py`

 * *Files 0% similar despite different names*

```diff
@@ -723,18 +723,16 @@
                     if color == "grayscale":
                         img = cv2.imread(data,cv2.IMREAD_GRAYSCALE)
                         img = np.expand_dims(img, 2)                 
                     else:
                         img = cv2.imread(data)
                     # img = np.array(Image.open(data))
                     transform = torch.load(checkpoint,map_location=torch.device('cpu'))['meta']['transform']
-                    print(img.shape,"+++")
                     if transform is not None:
                         img = np.array(transform(Image.fromarray(img)))
-                        print(img.shape)
                     data = torch.from_numpy(img).unsqueeze(0).permute(0,3,1,2).to(torch.float32).to(self.device) 
 
                     # if len(img.shape) == 2:
                     #     # 灰度，加两维度（sample，channel）
                     #     data = torch.from_numpy(img).unsqueeze(0).unsqueeze(0).to(torch.float32).to(self.device) 
                     # elif len(img.shape) == 3:
                     #     # 灰度/RGB，加一维度（sample）
@@ -783,16 +781,19 @@
                 self. res = res
                 return res
 
             else:  # 推理numpy数组
                 transform = torch.load(checkpoint,map_location=torch.device('cpu'))['meta']['transform']
                 if transform is not None:
                     data = np.array(transform(Image.fromarray(data)))
-                # data  = Variable(torch.tensor(np.array(data)).to(torch.float32)).to(self.device)
-                data = torch.from_numpy(data).unsqueeze(0).permute(0,3,1,2).to(torch.float32).to(self.device) 
+                if len(data.shape) == 3:
+                    data = torch.from_numpy(data).unsqueeze(0).permute(0,3,1,2).to(torch.float32).to(self.device) 
+                else:
+                    data  = Variable(torch.tensor(np.array(data)).to(torch.float32)).to(self.device)
+
 
             # print(data.shape)
             # data  = Variable(torch.tensor(np.array(data)))
             self.model = self.model.to(self.device)
             self.model.eval()
             with torch.no_grad():
                 res = self.model(data)
```

### Comparing `BaseNN-0.1.7/BaseNN/examples/BaseNN_demo.py` & `BaseNN-0.1.8/BaseNN/examples/BaseNN_demo.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from BaseNN import nn,pth_info
 # import torch
 import numpy as np
 import cv2
 import os
+from tqdm import tqdm
+
 
 def cal_accuracy(y, pred_y):
     res = pred_y.argmax(axis=1)
     print(res, y)
     tp = np.array(y)==np.array(res)
     acc = np.sum(tp)/ y.shape[0]
     return acc
@@ -480,26 +482,83 @@
     checkpoint = '111ckpt/basenn.pth'
     output, hidden = model.inference(data=input,checkpoint=checkpoint) # output是多维向量，接下来转化为汉字
     print("output: ",output)
     index = np.argmax(output) # 找到概率最大的字的索引
     w = model.ix2word[index] # 根据索引从词表中找到字
     print("word:",w)
 
-def txt2npz():
-    with open("tang.txt","r",encoding='utf-8') as f:
-        data = f.readlines()
-        data = [i.rstrip('\n') for i in data]
-        word2ix = {}
-        index = 1
-        for line in data:
-            for word in line:
-                pass
-        print(type(data),data)
+def npz2csv(npz_file,csv_file):
+    datas = np.load(npz_file,allow_pickle=True)
+    data = datas['data'] 
+    word2idx = datas['word2idx'].item() # 汉字对应的索引
+    idx2word = dict(zip(word2idx.values(),word2idx.keys()))
+    from tqdm import tqdm
+    import csv
+
+    with open(csv_file,'w') as f:
+        writer = csv.writer(f)
+        for line in tqdm(data):
+            verse = ""
+            for w in line:
+                if idx2word[w] not in ['</s>','<START>']:
+                    verse += idx2word[w]
+            writer.writerow([verse])
+    # np.savetxt("tangccc.csv",np.array(content),encoding='utf-8')
+
+def npz2txt(npz_file,txt_file):
+    datas = np.load(npz_file,allow_pickle=True)
+    data = datas['data'] 
+    print(data.shape)
+    # print("第一条数据：",data[0]) # 观察第一条数据
+    word2idx = datas['word2ix'].item() # 汉字对应的索引
+    idx2word = dict(zip(word2idx.values(),word2idx.keys()))
+    with open(txt_file,'w',encoding='utf-8') as f:
+        for line in tqdm(data):
+            verse = ""
+            for w in line:
+                if idx2word[w] not in ['</s>','<START>']:
+                    verse += idx2word[w]
+            f.write(verse +'\n')
+
+def txt2npz(txt_file,npz_file, token_size = 125):
+    with open(txt_file,'r') as f:
+        content = f.readlines()
+        content = [i.rstrip('\n') for i in content]
+        words = set() # 词表
+        for verse in content:
+            for w in verse:
+                words.add(w)
+        word2idx = {w:i for i,w in enumerate(words)}
+        start = len(words) + 1
+        # eop = len(words) + 2
+        s = len(words) +3
+        data = []
+        for verse in tqdm(content):
+            verse_l = [start]
+            for w in verse:
+                verse_l.append(word2idx[w])
+            # v_l.append(eop)
+            if len(verse_l) > token_size:
+                verse_l = verse_l[:token_size]
+            else:
+                for _ in range(token_size- len(verse_l)):
+                    verse_l.insert(0,s)
+            data.append(verse_l)
+        x, y = np.array(data)[:,:-1], np.array(data)[:, 1:]
+        print("词表大小：",len(words))
+        print("数据集大小：",x.shape[0])
+        np.savez(npz_file, data=x, label=y, word2idx=word2idx)
+        print("转化成功！保存为：",npz_file)
+
 
 if __name__=="__main__":
+    # npz2csv()
+    # npz2txt("tang.npz","tangccc.txt")
+
+    txt2npz("tangccc.txt","tangccc_n.npz")
     # load_npz_data_action()
     # load_npz_data_tang()
     # tang_infer()
     # txt2npz()
     # action_demo()
     # user_defined_demo()
     # data_define_demo()
@@ -518,9 +577,9 @@
     # extract_feature_demo()
 
     # lstm_train_demo()
     # pth_info('model_lstm.pth')
     # lstm_infer_demo()
 
     # load_image_data_mn()
-    load_image_data_cd()
+    # load_image_data_cd()
     # load_tab_data_iris()
```

### Comparing `BaseNN-0.1.7/BaseNN/examples/pkl2pth.py` & `BaseNN-0.1.8/BaseNN/examples/pkl2pth.py`

 * *Files identical despite different names*

### Comparing `BaseNN-0.1.7/BaseNN/load_data.py` & `BaseNN-0.1.8/BaseNN/load_data.py`

 * *Files identical despite different names*

### Comparing `BaseNN-0.1.7/BaseNN/version.py` & `BaseNN-0.1.8/BaseNN/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os
 
-__version__='0.1.7'
+__version__='0.1.8'
 __path__=os.path.abspath(os.getcwd())
 
 def parse_version_info(version_str):
     version_info = []
     for x in version_str.split('.'):
         if x.isdigit():
             version_info.append(int(x))
```

### Comparing `BaseNN-0.1.7/setup.py` & `BaseNN-0.1.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,15 +76,15 @@
 
     packages = list(gen_packages_items())
     return packages
 
 
 setup(
     name='BaseNN',
-    version='0.1.7',
+    version='0.1.8',
     description='BaseNN can easily build neural networks layer by layer and deeply explore the neural network principle.',
     license='MIT License',
     author='OpenXLab',
     author_email='wangbolun@pjlab.org.cn',
     url='https://github.com/OpenXLab-Edu/OpenMMLab-Edu',
     packages=find_packages(),
     include_package_data=True,
```

