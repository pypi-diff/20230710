# Comparing `tmp/baysalt_christmas-0.1.8.3.tar.gz` & `tmp/baysalt_christmas-0.1.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "baysalt_christmas-0.1.8.3.tar", last modified: Tue Jul  4 08:34:45 2023, max compression
+gzip compressed data, was "baysalt_christmas-0.1.8.4.tar", last modified: Mon Jul 10 06:35:22 2023, max compression
```

## Comparing `baysalt_christmas-0.1.8.3.tar` & `baysalt_christmas-0.1.8.4.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-07-04 08:34:45.649530 baysalt_christmas-0.1.8.3/
--rw-r--r--   0 christmas   (501) staff       (20)    10244 2023-06-13 08:58:02.000000 baysalt_christmas-0.1.8.3/.DS_Store
--rw-r--r--   0 christmas   (501) staff       (20)      117 2023-03-25 19:22:27.000000 baysalt_christmas-0.1.8.3/MANIFEST.in
--rw-r--r--   0 christmas   (501) staff       (20)     4095 2023-07-04 08:34:45.649367 baysalt_christmas-0.1.8.3/PKG-INFO
--rw-r--r--   0 christmas   (501) staff       (20)     3732 2023-03-29 03:30:38.000000 baysalt_christmas-0.1.8.3/README.md
-drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-07-04 08:34:45.640874 baysalt_christmas-0.1.8.3/baysalt_christmas.egg-info/
--rw-r--r--   0 christmas   (501) staff       (20)     4095 2023-07-04 08:34:45.000000 baysalt_christmas-0.1.8.3/baysalt_christmas.egg-info/PKG-INFO
--rw-r--r--   0 christmas   (501) staff       (20)      788 2023-07-04 08:34:45.000000 baysalt_christmas-0.1.8.3/baysalt_christmas.egg-info/SOURCES.txt
--rw-r--r--   0 christmas   (501) staff       (20)        1 2023-07-04 08:34:45.000000 baysalt_christmas-0.1.8.3/baysalt_christmas.egg-info/dependency_links.txt
--rw-r--r--   0 christmas   (501) staff       (20)       30 2023-07-04 08:34:45.000000 baysalt_christmas-0.1.8.3/baysalt_christmas.egg-info/requires.txt
--rw-r--r--   0 christmas   (501) staff       (20)       10 2023-07-04 08:34:45.000000 baysalt_christmas-0.1.8.3/baysalt_christmas.egg-info/top_level.txt
-drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-07-04 08:34:45.643889 baysalt_christmas-0.1.8.3/christmas/
--rw-r--r--   0 christmas   (501) staff       (20)    21061 2023-06-08 02:22:25.000000 baysalt_christmas-0.1.8.3/christmas/Blogging.py
-drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-07-04 08:34:45.644675 baysalt_christmas-0.1.8.3/christmas/Pyshell/
--rw-r--r--   0 christmas   (501) staff       (20)     5957 2023-07-04 08:34:25.000000 baysalt_christmas-0.1.8.3/christmas/Pyshell/RS_File.py
--rw-r--r--   0 christmas   (501) staff       (20)      249 2023-07-03 02:25:19.000000 baysalt_christmas-0.1.8.3/christmas/Pyshell/__init__.py
--rw-r--r--   0 christmas   (501) staff       (20)     1895 2023-03-25 02:55:02.000000 baysalt_christmas-0.1.8.3/christmas/S_DateTime.py
--rw-r--r--   0 christmas   (501) staff       (20)      405 2023-07-03 02:25:27.000000 baysalt_christmas-0.1.8.3/christmas/__init__.py
--rw-r--r--   0 christmas   (501) staff       (20)     4676 2023-05-17 09:02:10.000000 baysalt_christmas-0.1.8.3/christmas/commonCode.py
--rw-r--r--   0 christmas   (501) staff       (20)     1638 2023-04-12 07:23:55.000000 baysalt_christmas-0.1.8.3/christmas/cprintf.py
-drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-07-04 08:34:45.647736 baysalt_christmas-0.1.8.3/christmas/mncPy/
--rw-r--r--   0 christmas   (501) staff       (20)     1203 2023-03-03 04:53:20.000000 baysalt_christmas-0.1.8.3/christmas/mncPy/.gitignore
--rw-r--r--   0 christmas   (501) staff       (20)    35149 2023-03-03 04:53:20.000000 baysalt_christmas-0.1.8.3/christmas/mncPy/LICENSE
--rw-r--r--   0 christmas   (501) staff       (20)      239 2023-03-03 08:53:41.000000 baysalt_christmas-0.1.8.3/christmas/mncPy/__init__.py
-drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-07-04 08:34:45.648959 baysalt_christmas-0.1.8.3/christmas/mncPy/__pycache__/
--rw-r--r--   0 christmas   (501) staff       (20)      228 2023-03-26 18:28:05.000000 baysalt_christmas-0.1.8.3/christmas/mncPy/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 christmas   (501) staff       (20)     8964 2023-04-08 09:55:17.000000 baysalt_christmas-0.1.8.3/christmas/mncPy/__pycache__/common.cpython-39.pyc
--rw-r--r--   0 christmas   (501) staff       (20)     3411 2023-04-08 09:55:17.000000 baysalt_christmas-0.1.8.3/christmas/mncPy/__pycache__/compress.cpython-39.pyc
--rw-r--r--   0 christmas   (501) staff       (20)    12920 2023-03-09 13:49:40.000000 baysalt_christmas-0.1.8.3/christmas/mncPy/common.py
--rw-r--r--   0 christmas   (501) staff       (20)     4347 2023-03-09 14:00:22.000000 baysalt_christmas-0.1.8.3/christmas/mncPy/compress.py
--rw-r--r--   0 christmas   (501) staff       (20)     9042 2023-06-28 02:50:13.000000 baysalt_christmas-0.1.8.3/christmas/processBar.py
--rw-r--r--   0 christmas   (501) staff       (20)     3679 2023-06-12 03:11:04.000000 baysalt_christmas-0.1.8.3/christmas/read_conf.py
--rw-r--r--   0 christmas   (501) staff       (20)     1506 2022-12-07 09:44:40.000000 baysalt_christmas-0.1.8.3/christmas/server_info.py
--rw-r--r--   0 christmas   (501) staff       (20)      456 2023-03-25 18:44:30.000000 baysalt_christmas-0.1.8.3/run_twine.py
--rw-r--r--   0 christmas   (501) staff       (20)       38 2023-07-04 08:34:45.649586 baysalt_christmas-0.1.8.3/setup.cfg
--rw-r--r--   0 christmas   (501) staff       (20)      796 2023-07-04 08:34:43.000000 baysalt_christmas-0.1.8.3/setup.py
+drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-07-10 06:35:22.576160 baysalt_christmas-0.1.8.4/
+-rw-r--r--   0 christmas   (501) staff       (20)    10244 2023-06-13 08:58:02.000000 baysalt_christmas-0.1.8.4/.DS_Store
+-rw-r--r--   0 christmas   (501) staff       (20)      117 2023-03-25 19:22:27.000000 baysalt_christmas-0.1.8.4/MANIFEST.in
+-rw-r--r--   0 christmas   (501) staff       (20)     4095 2023-07-10 06:35:22.576008 baysalt_christmas-0.1.8.4/PKG-INFO
+-rw-r--r--   0 christmas   (501) staff       (20)     3732 2023-03-29 03:30:38.000000 baysalt_christmas-0.1.8.4/README.md
+drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-07-10 06:35:22.568596 baysalt_christmas-0.1.8.4/baysalt_christmas.egg-info/
+-rw-r--r--   0 christmas   (501) staff       (20)     4095 2023-07-10 06:35:22.000000 baysalt_christmas-0.1.8.4/baysalt_christmas.egg-info/PKG-INFO
+-rw-r--r--   0 christmas   (501) staff       (20)      788 2023-07-10 06:35:22.000000 baysalt_christmas-0.1.8.4/baysalt_christmas.egg-info/SOURCES.txt
+-rw-r--r--   0 christmas   (501) staff       (20)        1 2023-07-10 06:35:22.000000 baysalt_christmas-0.1.8.4/baysalt_christmas.egg-info/dependency_links.txt
+-rw-r--r--   0 christmas   (501) staff       (20)       30 2023-07-10 06:35:22.000000 baysalt_christmas-0.1.8.4/baysalt_christmas.egg-info/requires.txt
+-rw-r--r--   0 christmas   (501) staff       (20)       10 2023-07-10 06:35:22.000000 baysalt_christmas-0.1.8.4/baysalt_christmas.egg-info/top_level.txt
+drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-07-10 06:35:22.571199 baysalt_christmas-0.1.8.4/christmas/
+-rw-r--r--   0 christmas   (501) staff       (20)    21061 2023-06-08 02:22:25.000000 baysalt_christmas-0.1.8.4/christmas/Blogging.py
+drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-07-10 06:35:22.571725 baysalt_christmas-0.1.8.4/christmas/Pyshell/
+-rw-r--r--   0 christmas   (501) staff       (20)     5957 2023-07-04 08:34:25.000000 baysalt_christmas-0.1.8.4/christmas/Pyshell/RS_File.py
+-rw-r--r--   0 christmas   (501) staff       (20)      249 2023-07-03 02:25:19.000000 baysalt_christmas-0.1.8.4/christmas/Pyshell/__init__.py
+-rw-r--r--   0 christmas   (501) staff       (20)     1895 2023-03-25 02:55:02.000000 baysalt_christmas-0.1.8.4/christmas/S_DateTime.py
+-rw-r--r--   0 christmas   (501) staff       (20)      405 2023-07-03 02:25:27.000000 baysalt_christmas-0.1.8.4/christmas/__init__.py
+-rw-r--r--   0 christmas   (501) staff       (20)     4676 2023-05-17 09:02:10.000000 baysalt_christmas-0.1.8.4/christmas/commonCode.py
+-rw-r--r--   0 christmas   (501) staff       (20)     1638 2023-04-12 07:23:55.000000 baysalt_christmas-0.1.8.4/christmas/cprintf.py
+drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-07-10 06:35:22.574226 baysalt_christmas-0.1.8.4/christmas/mncPy/
+-rw-r--r--   0 christmas   (501) staff       (20)     1203 2023-03-03 04:53:20.000000 baysalt_christmas-0.1.8.4/christmas/mncPy/.gitignore
+-rw-r--r--   0 christmas   (501) staff       (20)    35149 2023-03-03 04:53:20.000000 baysalt_christmas-0.1.8.4/christmas/mncPy/LICENSE
+-rw-r--r--   0 christmas   (501) staff       (20)      239 2023-03-03 08:53:41.000000 baysalt_christmas-0.1.8.4/christmas/mncPy/__init__.py
+drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-07-10 06:35:22.575622 baysalt_christmas-0.1.8.4/christmas/mncPy/__pycache__/
+-rw-r--r--   0 christmas   (501) staff       (20)      228 2023-03-26 18:28:05.000000 baysalt_christmas-0.1.8.4/christmas/mncPy/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 christmas   (501) staff       (20)     8964 2023-04-08 09:55:17.000000 baysalt_christmas-0.1.8.4/christmas/mncPy/__pycache__/common.cpython-39.pyc
+-rw-r--r--   0 christmas   (501) staff       (20)     3411 2023-04-08 09:55:17.000000 baysalt_christmas-0.1.8.4/christmas/mncPy/__pycache__/compress.cpython-39.pyc
+-rw-r--r--   0 christmas   (501) staff       (20)    12920 2023-03-09 13:49:40.000000 baysalt_christmas-0.1.8.4/christmas/mncPy/common.py
+-rw-r--r--   0 christmas   (501) staff       (20)     4347 2023-03-09 14:00:22.000000 baysalt_christmas-0.1.8.4/christmas/mncPy/compress.py
+-rw-r--r--   0 christmas   (501) staff       (20)     9134 2023-07-10 06:35:18.000000 baysalt_christmas-0.1.8.4/christmas/processBar.py
+-rw-r--r--   0 christmas   (501) staff       (20)     3679 2023-06-12 03:11:04.000000 baysalt_christmas-0.1.8.4/christmas/read_conf.py
+-rw-r--r--   0 christmas   (501) staff       (20)     1506 2022-12-07 09:44:40.000000 baysalt_christmas-0.1.8.4/christmas/server_info.py
+-rw-r--r--   0 christmas   (501) staff       (20)      456 2023-03-25 18:44:30.000000 baysalt_christmas-0.1.8.4/run_twine.py
+-rw-r--r--   0 christmas   (501) staff       (20)       38 2023-07-10 06:35:22.576220 baysalt_christmas-0.1.8.4/setup.cfg
+-rw-r--r--   0 christmas   (501) staff       (20)      796 2023-07-10 06:35:18.000000 baysalt_christmas-0.1.8.4/setup.py
```

### Comparing `baysalt_christmas-0.1.8.3/.DS_Store` & `baysalt_christmas-0.1.8.4/.DS_Store`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.8.3/PKG-INFO` & `baysalt_christmas-0.1.8.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: baysalt_christmas
-Version: 0.1.8.3
+Version: 0.1.8.4
 Summary: Some simple tools for Christmas
 Author: Christmas
 Author-email: 273519355@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `baysalt_christmas-0.1.8.3/README.md` & `baysalt_christmas-0.1.8.4/README.md`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.8.3/baysalt_christmas.egg-info/PKG-INFO` & `baysalt_christmas-0.1.8.4/baysalt_christmas.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: baysalt-christmas
-Version: 0.1.8.3
+Version: 0.1.8.4
 Summary: Some simple tools for Christmas
 Author: Christmas
 Author-email: 273519355@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `baysalt_christmas-0.1.8.3/baysalt_christmas.egg-info/SOURCES.txt` & `baysalt_christmas-0.1.8.4/baysalt_christmas.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.8.3/christmas/Blogging.py` & `baysalt_christmas-0.1.8.4/christmas/Blogging.py`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.8.3/christmas/Pyshell/RS_File.py` & `baysalt_christmas-0.1.8.4/christmas/Pyshell/RS_File.py`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.8.3/christmas/S_DateTime.py` & `baysalt_christmas-0.1.8.4/christmas/S_DateTime.py`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.8.3/christmas/commonCode.py` & `baysalt_christmas-0.1.8.4/christmas/commonCode.py`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.8.3/christmas/cprintf.py` & `baysalt_christmas-0.1.8.4/christmas/cprintf.py`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.8.3/christmas/mncPy/.gitignore` & `baysalt_christmas-0.1.8.4/christmas/mncPy/.gitignore`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.8.3/christmas/mncPy/LICENSE` & `baysalt_christmas-0.1.8.4/christmas/mncPy/LICENSE`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.8.3/christmas/mncPy/__pycache__/common.cpython-39.pyc` & `baysalt_christmas-0.1.8.4/christmas/mncPy/__pycache__/common.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.8.3/christmas/mncPy/__pycache__/compress.cpython-39.pyc` & `baysalt_christmas-0.1.8.4/christmas/mncPy/__pycache__/compress.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.8.3/christmas/mncPy/common.py` & `baysalt_christmas-0.1.8.4/christmas/mncPy/common.py`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.8.3/christmas/mncPy/compress.py` & `baysalt_christmas-0.1.8.4/christmas/mncPy/compress.py`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.8.3/christmas/processBar.py` & `baysalt_christmas-0.1.8.4/christmas/processBar.py`

 * *Files 2% similar despite different names*

```diff
@@ -214,28 +214,30 @@
 		self.sizeWritten = 0                       # 已上传或下载大小
 		self.lastShownPercent = 0                  # 上次显示的百分比
 		self.lastNum = 0                           # 低速的次数
 		self.exit_num = exit_num                   # 退出次数
 		self.bar_length = bar_length               # 进度条长度
 		self.change_percent = change_percent       # 进度条变化百分比 0为1%输出 1为0.1%输出 2为0.01%输出
 		self.INFO = INFO                           # 是否显示进度条信息
+		self.speed_list = []                       # 速度列表
 		if fp:
 			self.fp = fp                           # 文件对象
 
 	def callback_html(self, block):
 		"""
 		:param block: 上传或下载的数据块
 		"""
 		if self.fp:
 			self.fp.write(block)
 		self.sizeWritten += len(block)
 		percents = '\033[32;1m%s\033[0m' % round(float(self.sizeWritten) * 100 / float(self.totalSize), self.change_percent)
 		filled = int(self.bar_length * self.sizeWritten / float(self.totalSize))
 		bar = '\033[32;1m%s\033[0m' % '=' * filled + '-' * (self.bar_length - filled)
 		speed = self.sizeWritten / (np.float64(time.time()) - self.time_start)
+		self.speed_list.append(speed)
 
 		percentComplete = round((self.sizeWritten / self.totalSize) * 100, self.change_percent)  # 粗分辨率,防止刷新过快
 		if self.lastShownPercent != percentComplete:
 			self.lastShownPercent = percentComplete
 			if self.INFO:
 				ddt = datetime.datetime.now().strftime('%Y-%m-%d %H:%M:%S')
 				print('\r'+f'{ddt} ---> [{bar}] {percents}% speed:{translate_byte(speed)}/s, already complete: {translate_byte(self.sizeWritten)}, total: {translate_byte(self.totalSize)}', end='')
```

### Comparing `baysalt_christmas-0.1.8.3/christmas/read_conf.py` & `baysalt_christmas-0.1.8.4/christmas/read_conf.py`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.8.3/christmas/server_info.py` & `baysalt_christmas-0.1.8.4/christmas/server_info.py`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.8.3/setup.py` & `baysalt_christmas-0.1.8.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 setuptools.setup(
     name="baysalt_christmas",
-    version="0.1.8.3",
+    version="0.1.8.4",
     author="Christmas",
     author_email="273519355@qq.com",
     description="Some simple tools for Christmas",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     include_package_data=True,
```

