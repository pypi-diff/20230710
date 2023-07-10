# Comparing `tmp/baysalt_christmas-0.1.8.4.tar.gz` & `tmp/baysalt_christmas-0.1.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "baysalt_christmas-0.1.8.4.tar", last modified: Mon Jul 10 06:35:22 2023, max compression
+gzip compressed data, was "baysalt_christmas-0.1.8.5.tar", last modified: Mon Jul 10 06:54:35 2023, max compression
```

## Comparing `baysalt_christmas-0.1.8.4.tar` & `baysalt_christmas-0.1.8.5.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-07-10 06:35:22.576160 baysalt_christmas-0.1.8.4/
--rw-r--r--   0 christmas   (501) staff       (20)    10244 2023-06-13 08:58:02.000000 baysalt_christmas-0.1.8.4/.DS_Store
--rw-r--r--   0 christmas   (501) staff       (20)      117 2023-03-25 19:22:27.000000 baysalt_christmas-0.1.8.4/MANIFEST.in
--rw-r--r--   0 christmas   (501) staff       (20)     4095 2023-07-10 06:35:22.576008 baysalt_christmas-0.1.8.4/PKG-INFO
--rw-r--r--   0 christmas   (501) staff       (20)     3732 2023-03-29 03:30:38.000000 baysalt_christmas-0.1.8.4/README.md
-drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-07-10 06:35:22.568596 baysalt_christmas-0.1.8.4/baysalt_christmas.egg-info/
--rw-r--r--   0 christmas   (501) staff       (20)     4095 2023-07-10 06:35:22.000000 baysalt_christmas-0.1.8.4/baysalt_christmas.egg-info/PKG-INFO
--rw-r--r--   0 christmas   (501) staff       (20)      788 2023-07-10 06:35:22.000000 baysalt_christmas-0.1.8.4/baysalt_christmas.egg-info/SOURCES.txt
--rw-r--r--   0 christmas   (501) staff       (20)        1 2023-07-10 06:35:22.000000 baysalt_christmas-0.1.8.4/baysalt_christmas.egg-info/dependency_links.txt
--rw-r--r--   0 christmas   (501) staff       (20)       30 2023-07-10 06:35:22.000000 baysalt_christmas-0.1.8.4/baysalt_christmas.egg-info/requires.txt
--rw-r--r--   0 christmas   (501) staff       (20)       10 2023-07-10 06:35:22.000000 baysalt_christmas-0.1.8.4/baysalt_christmas.egg-info/top_level.txt
-drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-07-10 06:35:22.571199 baysalt_christmas-0.1.8.4/christmas/
--rw-r--r--   0 christmas   (501) staff       (20)    21061 2023-06-08 02:22:25.000000 baysalt_christmas-0.1.8.4/christmas/Blogging.py
-drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-07-10 06:35:22.571725 baysalt_christmas-0.1.8.4/christmas/Pyshell/
--rw-r--r--   0 christmas   (501) staff       (20)     5957 2023-07-04 08:34:25.000000 baysalt_christmas-0.1.8.4/christmas/Pyshell/RS_File.py
--rw-r--r--   0 christmas   (501) staff       (20)      249 2023-07-03 02:25:19.000000 baysalt_christmas-0.1.8.4/christmas/Pyshell/__init__.py
--rw-r--r--   0 christmas   (501) staff       (20)     1895 2023-03-25 02:55:02.000000 baysalt_christmas-0.1.8.4/christmas/S_DateTime.py
--rw-r--r--   0 christmas   (501) staff       (20)      405 2023-07-03 02:25:27.000000 baysalt_christmas-0.1.8.4/christmas/__init__.py
--rw-r--r--   0 christmas   (501) staff       (20)     4676 2023-05-17 09:02:10.000000 baysalt_christmas-0.1.8.4/christmas/commonCode.py
--rw-r--r--   0 christmas   (501) staff       (20)     1638 2023-04-12 07:23:55.000000 baysalt_christmas-0.1.8.4/christmas/cprintf.py
-drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-07-10 06:35:22.574226 baysalt_christmas-0.1.8.4/christmas/mncPy/
--rw-r--r--   0 christmas   (501) staff       (20)     1203 2023-03-03 04:53:20.000000 baysalt_christmas-0.1.8.4/christmas/mncPy/.gitignore
--rw-r--r--   0 christmas   (501) staff       (20)    35149 2023-03-03 04:53:20.000000 baysalt_christmas-0.1.8.4/christmas/mncPy/LICENSE
--rw-r--r--   0 christmas   (501) staff       (20)      239 2023-03-03 08:53:41.000000 baysalt_christmas-0.1.8.4/christmas/mncPy/__init__.py
-drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-07-10 06:35:22.575622 baysalt_christmas-0.1.8.4/christmas/mncPy/__pycache__/
--rw-r--r--   0 christmas   (501) staff       (20)      228 2023-03-26 18:28:05.000000 baysalt_christmas-0.1.8.4/christmas/mncPy/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 christmas   (501) staff       (20)     8964 2023-04-08 09:55:17.000000 baysalt_christmas-0.1.8.4/christmas/mncPy/__pycache__/common.cpython-39.pyc
--rw-r--r--   0 christmas   (501) staff       (20)     3411 2023-04-08 09:55:17.000000 baysalt_christmas-0.1.8.4/christmas/mncPy/__pycache__/compress.cpython-39.pyc
--rw-r--r--   0 christmas   (501) staff       (20)    12920 2023-03-09 13:49:40.000000 baysalt_christmas-0.1.8.4/christmas/mncPy/common.py
--rw-r--r--   0 christmas   (501) staff       (20)     4347 2023-03-09 14:00:22.000000 baysalt_christmas-0.1.8.4/christmas/mncPy/compress.py
--rw-r--r--   0 christmas   (501) staff       (20)     9134 2023-07-10 06:35:18.000000 baysalt_christmas-0.1.8.4/christmas/processBar.py
--rw-r--r--   0 christmas   (501) staff       (20)     3679 2023-06-12 03:11:04.000000 baysalt_christmas-0.1.8.4/christmas/read_conf.py
--rw-r--r--   0 christmas   (501) staff       (20)     1506 2022-12-07 09:44:40.000000 baysalt_christmas-0.1.8.4/christmas/server_info.py
--rw-r--r--   0 christmas   (501) staff       (20)      456 2023-03-25 18:44:30.000000 baysalt_christmas-0.1.8.4/run_twine.py
--rw-r--r--   0 christmas   (501) staff       (20)       38 2023-07-10 06:35:22.576220 baysalt_christmas-0.1.8.4/setup.cfg
--rw-r--r--   0 christmas   (501) staff       (20)      796 2023-07-10 06:35:18.000000 baysalt_christmas-0.1.8.4/setup.py
+drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-07-10 06:54:35.110879 baysalt_christmas-0.1.8.5/
+-rw-r--r--   0 christmas   (501) staff       (20)    10244 2023-06-13 08:58:02.000000 baysalt_christmas-0.1.8.5/.DS_Store
+-rw-r--r--   0 christmas   (501) staff       (20)      117 2023-03-25 19:22:27.000000 baysalt_christmas-0.1.8.5/MANIFEST.in
+-rw-r--r--   0 christmas   (501) staff       (20)     4095 2023-07-10 06:54:35.110723 baysalt_christmas-0.1.8.5/PKG-INFO
+-rw-r--r--   0 christmas   (501) staff       (20)     3732 2023-03-29 03:30:38.000000 baysalt_christmas-0.1.8.5/README.md
+drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-07-10 06:54:35.101476 baysalt_christmas-0.1.8.5/baysalt_christmas.egg-info/
+-rw-r--r--   0 christmas   (501) staff       (20)     4095 2023-07-10 06:54:35.000000 baysalt_christmas-0.1.8.5/baysalt_christmas.egg-info/PKG-INFO
+-rw-r--r--   0 christmas   (501) staff       (20)      788 2023-07-10 06:54:35.000000 baysalt_christmas-0.1.8.5/baysalt_christmas.egg-info/SOURCES.txt
+-rw-r--r--   0 christmas   (501) staff       (20)        1 2023-07-10 06:54:35.000000 baysalt_christmas-0.1.8.5/baysalt_christmas.egg-info/dependency_links.txt
+-rw-r--r--   0 christmas   (501) staff       (20)       30 2023-07-10 06:54:35.000000 baysalt_christmas-0.1.8.5/baysalt_christmas.egg-info/requires.txt
+-rw-r--r--   0 christmas   (501) staff       (20)       10 2023-07-10 06:54:35.000000 baysalt_christmas-0.1.8.5/baysalt_christmas.egg-info/top_level.txt
+drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-07-10 06:54:35.104076 baysalt_christmas-0.1.8.5/christmas/
+-rw-r--r--   0 christmas   (501) staff       (20)    21061 2023-06-08 02:22:25.000000 baysalt_christmas-0.1.8.5/christmas/Blogging.py
+drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-07-10 06:54:35.104682 baysalt_christmas-0.1.8.5/christmas/Pyshell/
+-rw-r--r--   0 christmas   (501) staff       (20)     5957 2023-07-04 08:34:25.000000 baysalt_christmas-0.1.8.5/christmas/Pyshell/RS_File.py
+-rw-r--r--   0 christmas   (501) staff       (20)      249 2023-07-03 02:25:19.000000 baysalt_christmas-0.1.8.5/christmas/Pyshell/__init__.py
+-rw-r--r--   0 christmas   (501) staff       (20)     1895 2023-03-25 02:55:02.000000 baysalt_christmas-0.1.8.5/christmas/S_DateTime.py
+-rw-r--r--   0 christmas   (501) staff       (20)      405 2023-07-03 02:25:27.000000 baysalt_christmas-0.1.8.5/christmas/__init__.py
+-rw-r--r--   0 christmas   (501) staff       (20)     4676 2023-05-17 09:02:10.000000 baysalt_christmas-0.1.8.5/christmas/commonCode.py
+-rw-r--r--   0 christmas   (501) staff       (20)     1638 2023-04-12 07:23:55.000000 baysalt_christmas-0.1.8.5/christmas/cprintf.py
+drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-07-10 06:54:35.109516 baysalt_christmas-0.1.8.5/christmas/mncPy/
+-rw-r--r--   0 christmas   (501) staff       (20)     1203 2023-03-03 04:53:20.000000 baysalt_christmas-0.1.8.5/christmas/mncPy/.gitignore
+-rw-r--r--   0 christmas   (501) staff       (20)    35149 2023-03-03 04:53:20.000000 baysalt_christmas-0.1.8.5/christmas/mncPy/LICENSE
+-rw-r--r--   0 christmas   (501) staff       (20)      239 2023-03-03 08:53:41.000000 baysalt_christmas-0.1.8.5/christmas/mncPy/__init__.py
+drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-07-10 06:54:35.110371 baysalt_christmas-0.1.8.5/christmas/mncPy/__pycache__/
+-rw-r--r--   0 christmas   (501) staff       (20)      228 2023-03-26 18:28:05.000000 baysalt_christmas-0.1.8.5/christmas/mncPy/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 christmas   (501) staff       (20)     8964 2023-04-08 09:55:17.000000 baysalt_christmas-0.1.8.5/christmas/mncPy/__pycache__/common.cpython-39.pyc
+-rw-r--r--   0 christmas   (501) staff       (20)     3411 2023-04-08 09:55:17.000000 baysalt_christmas-0.1.8.5/christmas/mncPy/__pycache__/compress.cpython-39.pyc
+-rw-r--r--   0 christmas   (501) staff       (20)    12920 2023-03-09 13:49:40.000000 baysalt_christmas-0.1.8.5/christmas/mncPy/common.py
+-rw-r--r--   0 christmas   (501) staff       (20)     4347 2023-03-09 14:00:22.000000 baysalt_christmas-0.1.8.5/christmas/mncPy/compress.py
+-rw-r--r--   0 christmas   (501) staff       (20)     9260 2023-07-10 06:49:33.000000 baysalt_christmas-0.1.8.5/christmas/processBar.py
+-rw-r--r--   0 christmas   (501) staff       (20)     3679 2023-06-12 03:11:04.000000 baysalt_christmas-0.1.8.5/christmas/read_conf.py
+-rw-r--r--   0 christmas   (501) staff       (20)     1506 2022-12-07 09:44:40.000000 baysalt_christmas-0.1.8.5/christmas/server_info.py
+-rw-r--r--   0 christmas   (501) staff       (20)      456 2023-03-25 18:44:30.000000 baysalt_christmas-0.1.8.5/run_twine.py
+-rw-r--r--   0 christmas   (501) staff       (20)       38 2023-07-10 06:54:35.110934 baysalt_christmas-0.1.8.5/setup.cfg
+-rw-r--r--   0 christmas   (501) staff       (20)      796 2023-07-10 06:54:31.000000 baysalt_christmas-0.1.8.5/setup.py
```

### Comparing `baysalt_christmas-0.1.8.4/.DS_Store` & `baysalt_christmas-0.1.8.5/.DS_Store`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.8.4/PKG-INFO` & `baysalt_christmas-0.1.8.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: baysalt_christmas
-Version: 0.1.8.4
+Version: 0.1.8.5
 Summary: Some simple tools for Christmas
 Author: Christmas
 Author-email: 273519355@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `baysalt_christmas-0.1.8.4/README.md` & `baysalt_christmas-0.1.8.5/README.md`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.8.4/baysalt_christmas.egg-info/PKG-INFO` & `baysalt_christmas-0.1.8.5/baysalt_christmas.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: baysalt-christmas
-Version: 0.1.8.4
+Version: 0.1.8.5
 Summary: Some simple tools for Christmas
 Author: Christmas
 Author-email: 273519355@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `baysalt_christmas-0.1.8.4/baysalt_christmas.egg-info/SOURCES.txt` & `baysalt_christmas-0.1.8.5/baysalt_christmas.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.8.4/christmas/Blogging.py` & `baysalt_christmas-0.1.8.5/christmas/Blogging.py`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.8.4/christmas/Pyshell/RS_File.py` & `baysalt_christmas-0.1.8.5/christmas/Pyshell/RS_File.py`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.8.4/christmas/S_DateTime.py` & `baysalt_christmas-0.1.8.5/christmas/S_DateTime.py`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.8.4/christmas/commonCode.py` & `baysalt_christmas-0.1.8.5/christmas/commonCode.py`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.8.4/christmas/cprintf.py` & `baysalt_christmas-0.1.8.5/christmas/cprintf.py`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.8.4/christmas/mncPy/.gitignore` & `baysalt_christmas-0.1.8.5/christmas/mncPy/.gitignore`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.8.4/christmas/mncPy/LICENSE` & `baysalt_christmas-0.1.8.5/christmas/mncPy/LICENSE`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.8.4/christmas/mncPy/__pycache__/common.cpython-39.pyc` & `baysalt_christmas-0.1.8.5/christmas/mncPy/__pycache__/common.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.8.4/christmas/mncPy/__pycache__/compress.cpython-39.pyc` & `baysalt_christmas-0.1.8.5/christmas/mncPy/__pycache__/compress.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.8.4/christmas/mncPy/common.py` & `baysalt_christmas-0.1.8.5/christmas/mncPy/common.py`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.8.4/christmas/mncPy/compress.py` & `baysalt_christmas-0.1.8.5/christmas/mncPy/compress.py`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.8.4/christmas/processBar.py` & `baysalt_christmas-0.1.8.5/christmas/processBar.py`

 * *Files 10% similar despite different names*

```diff
@@ -203,51 +203,51 @@
 		        for chunk in r.iter_content(chunksize):
 		            if chunk:
 		                Html_obj.callback_html(chunk)
 		except LowSpeed_Error as e:
 		    print(e.value)
 	"""
 
-	def __init__(self, totalSize, speed_min=512*1024, fp=None, exit_num=30, bar_length=30, change_percent=1, INFO=True):
-		self.totalSize = totalSize                 # 文件总大小
-		self.speed_min = speed_min                 # 上传或下载退出速度(单位是byte),默认512KB/s
-		self.time_start = np.float64(time.time())  # 开始上传或下载时间(注意是实例化时开始计时)
-		self.sizeWritten = 0                       # 已上传或下载大小
-		self.lastShownPercent = 0                  # 上次显示的百分比
-		self.lastNum = 0                           # 低速的次数
-		self.exit_num = exit_num                   # 退出次数
-		self.bar_length = bar_length               # 进度条长度
-		self.change_percent = change_percent       # 进度条变化百分比 0为1%输出 1为0.1%输出 2为0.01%输出
-		self.INFO = INFO                           # 是否显示进度条信息
-		self.speed_list = []                       # 速度列表
+	def __init__(self, totalSize, lowSpeed_floor=512*1024, fp=None, lowSpeed_exit_num=30, bar_length=30, change_percent=1, INFO=True):
+		self.totalSize = totalSize                        # 文件总大小
+		self.lowSpeed_floor = lowSpeed_floor              # 上传或下载退出速度(单位是byte),默认512KB/s
+		self.time_start = np.float64(time.time())         # 开始上传或下载时间(注意是实例化时开始计时)
+		self.sizeWritten = 0                              # 已上传或下载大小
+		self.__lastShownPercent = 0                       # 上次显示的百分比
+		self.lowSpeed_num = 0                             # 低速的次数
+		self.lowSpeed_exit_num = lowSpeed_exit_num  # 退出次数
+		self.__bar_length = bar_length                      # 进度条长度
+		self.change_percent = change_percent              # 进度条变化百分比 0为1%输出 1为0.1%输出 2为0.01%输出
+		self.INFO = INFO                                  # 是否显示进度条信息
+		self.speed_list = []                              # 速度列表
 		if fp:
-			self.fp = fp                           # 文件对象
+			self.fp = fp                                  # 文件对象
 
 	def callback_html(self, block):
 		"""
 		:param block: 上传或下载的数据块
 		"""
 		if self.fp:
 			self.fp.write(block)
 		self.sizeWritten += len(block)
 		percents = '\033[32;1m%s\033[0m' % round(float(self.sizeWritten) * 100 / float(self.totalSize), self.change_percent)
-		filled = int(self.bar_length * self.sizeWritten / float(self.totalSize))
-		bar = '\033[32;1m%s\033[0m' % '=' * filled + '-' * (self.bar_length - filled)
+		filled = int(self.__bar_length * self.sizeWritten / float(self.totalSize))
+		bar = '\033[32;1m%s\033[0m' % '=' * filled + '-' * (self.__bar_length - filled)
 		speed = self.sizeWritten / (np.float64(time.time()) - self.time_start)
 		self.speed_list.append(speed)
 
 		percentComplete = round((self.sizeWritten / self.totalSize) * 100, self.change_percent)  # 粗分辨率,防止刷新过快
-		if self.lastShownPercent != percentComplete:
-			self.lastShownPercent = percentComplete
+		if self.__lastShownPercent != percentComplete:
+			self.__lastShownPercent = percentComplete
 			if self.INFO:
 				ddt = datetime.datetime.now().strftime('%Y-%m-%d %H:%M:%S')
 				print('\r'+f'{ddt} ---> [{bar}] {percents}% speed:{translate_byte(speed)}/s, already complete: {translate_byte(self.sizeWritten)}, total: {translate_byte(self.totalSize)}', end='')
-		if speed < self.speed_min:
-			self.lastNum += 1
-			if self.lastNum >= self.exit_num and percentComplete <= 85:
+		if speed < self.lowSpeed_floor:
+			self.lowSpeed_num += 1
+			if self.lowSpeed_num >= self.lowSpeed_exit_num and percentComplete <= 85:
 				raise LowSpeed_Error(speed)
 
 	def callback_ftp(self):
 		"""
 		:return: 返回一个函数对象
 		"""
 		return self.callback_html
```

### Comparing `baysalt_christmas-0.1.8.4/christmas/read_conf.py` & `baysalt_christmas-0.1.8.5/christmas/read_conf.py`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.8.4/christmas/server_info.py` & `baysalt_christmas-0.1.8.5/christmas/server_info.py`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.8.4/setup.py` & `baysalt_christmas-0.1.8.5/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 setuptools.setup(
     name="baysalt_christmas",
-    version="0.1.8.4",
+    version="0.1.8.5",
     author="Christmas",
     author_email="273519355@qq.com",
     description="Some simple tools for Christmas",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     include_package_data=True,
```

