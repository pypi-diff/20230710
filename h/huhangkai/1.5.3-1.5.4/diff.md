# Comparing `tmp/huhangkai-1.5.3.tar.gz` & `tmp/huhangkai-1.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "huhangkai-1.5.3.tar", last modified: Fri Jul  7 08:33:19 2023, max compression
+gzip compressed data, was "huhangkai-1.5.4.tar", last modified: Mon Jul 10 07:58:04 2023, max compression
```

## Comparing `huhangkai-1.5.3.tar` & `huhangkai-1.5.4.tar`

### file list

```diff
@@ -1,44 +1,45 @@
-drwxrwxrwx   0        0        0        0 2023-07-07 08:33:19.807334 huhangkai-1.5.3/
--rw-rw-rw-   0        0        0      228 2023-07-07 08:33:19.806337 huhangkai-1.5.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-07 08:33:19.755473 huhangkai-1.5.3/commen/
--rw-rw-rw-   0        0        0      933 2023-07-05 02:58:25.000000 huhangkai-1.5.3/commen/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-07 08:33:19.765446 huhangkai-1.5.3/commen/case_project/
--rw-rw-rw-   0        0        0        0 2023-07-05 02:58:25.000000 huhangkai-1.5.3/commen/case_project/__init__.py
--rw-rw-rw-   0        0        0     3080 2023-07-05 02:58:25.000000 huhangkai-1.5.3/commen/case_project/base_project.py
--rw-rw-rw-   0        0        0      639 2023-07-05 09:37:54.000000 huhangkai-1.5.3/commen/case_project/json_coder.py
--rw-rw-rw-   0        0        0      822 2023-07-05 06:26:21.000000 huhangkai-1.5.3/commen/case_project/setup_set.py
--rw-rw-rw-   0        0        0       17 2023-07-07 08:33:19.000000 huhangkai-1.5.3/commen/case_project/version.py
--rw-rw-rw-   0        0        0    29301 2023-07-05 02:58:25.000000 huhangkai-1.5.3/commen/init_project.py
--rw-rw-rw-   0        0        0      276 2023-07-05 02:58:25.000000 huhangkai-1.5.3/commen/setup_run.py
-drwxrwxrwx   0        0        0        0 2023-07-07 08:33:19.767441 huhangkai-1.5.3/commen/testcase/
--rw-rw-rw-   0        0        0        0 2023-07-05 02:58:25.000000 huhangkai-1.5.3/commen/testcase/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-07 08:33:19.796364 huhangkai-1.5.3/commen/testcase/apache/
--rw-rw-rw-   0        0        0        0 2023-07-05 02:58:25.000000 huhangkai-1.5.3/commen/testcase/apache/__init__.py
--rw-rw-rw-   0        0        0     3355 2023-07-05 02:58:25.000000 huhangkai-1.5.3/commen/testcase/apache/beam_class.py
--rw-rw-rw-   0        0        0     5523 2023-07-05 02:58:25.000000 huhangkai-1.5.3/commen/testcase/apache/data.py
--rw-rw-rw-   0        0        0     1764 2023-07-05 02:58:25.000000 huhangkai-1.5.3/commen/testcase/apache/par_do.py
--rw-rw-rw-   0        0        0     7080 2023-07-05 02:58:25.000000 huhangkai-1.5.3/commen/testcase/apache/test_cogroupbykey.py
--rw-rw-rw-   0        0        0      521 2023-07-05 08:50:31.000000 huhangkai-1.5.3/commen/testcase/apache/test_file.py
--rw-rw-rw-   0        0        0     1548 2023-07-05 02:58:25.000000 huhangkai-1.5.3/commen/testcase/apache/test_fiter.py
--rw-rw-rw-   0        0        0     2148 2023-07-05 02:58:25.000000 huhangkai-1.5.3/commen/testcase/apache/test_flatmap.py
--rw-rw-rw-   0        0        0      568 2023-07-05 02:58:25.000000 huhangkai-1.5.3/commen/testcase/apache/test_map.py
--rw-rw-rw-   0        0        0     2621 2023-07-05 02:58:25.000000 huhangkai-1.5.3/commen/testcase/apache/test_par_do.py
--rw-rw-rw-   0        0        0     1696 2023-07-05 02:58:25.000000 huhangkai-1.5.3/commen/testcase/apache/test_regex.py
--rw-rw-rw-   0        0        0      519 2023-07-05 02:58:25.000000 huhangkai-1.5.3/commen/testcase/apache/test_time.py
--rw-rw-rw-   0        0        0      553 2023-07-05 02:58:25.000000 huhangkai-1.5.3/commen/testcase/apache/test_to_string.py
--rw-rw-rw-   0        0        0    21837 2023-07-05 10:01:08.000000 huhangkai-1.5.3/commen/unit_apache_beam.py
--rw-rw-rw-   0        0        0     4508 2023-07-05 02:58:25.000000 huhangkai-1.5.3/commen/unit_dict.py
--rw-rw-rw-   0        0        0     3843 2023-07-05 02:58:25.000000 huhangkai-1.5.3/commen/unit_encryption.py
--rw-rw-rw-   0        0        0    24880 2023-07-07 08:33:07.000000 huhangkai-1.5.3/commen/unit_fun.py
--rw-rw-rw-   0        0        0     1242 2023-07-05 02:58:25.000000 huhangkai-1.5.3/commen/unit_logger.py
--rw-rw-rw-   0        0        0     9218 2023-07-05 02:58:25.000000 huhangkai-1.5.3/commen/unit_request.py
--rw-rw-rw-   0        0        0     2473 2023-07-05 02:58:25.000000 huhangkai-1.5.3/commen/unit_tasks.py
--rw-rw-rw-   0        0        0      733 2023-07-05 02:58:25.000000 huhangkai-1.5.3/commen/常用命令.py
-drwxrwxrwx   0        0        0        0 2023-07-07 08:33:19.804342 huhangkai-1.5.3/huhangkai.egg-info/
--rw-rw-rw-   0        0        0      228 2023-07-07 08:33:19.000000 huhangkai-1.5.3/huhangkai.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1088 2023-07-07 08:33:19.000000 huhangkai-1.5.3/huhangkai.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-07 08:33:19.000000 huhangkai-1.5.3/huhangkai.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      128 2023-07-07 08:33:19.000000 huhangkai-1.5.3/huhangkai.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-07 08:33:19.000000 huhangkai-1.5.3/huhangkai.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-07 08:33:19.807334 huhangkai-1.5.3/setup.cfg
--rw-rw-rw-   0        0        0        2 2023-07-03 11:51:22.000000 huhangkai-1.5.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-10 07:58:04.923114 huhangkai-1.5.4/
+-rw-rw-rw-   0        0        0      228 2023-07-10 07:58:04.922116 huhangkai-1.5.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-10 07:58:04.853299 huhangkai-1.5.4/commen/
+-rw-rw-rw-   0        0        0      933 2023-07-05 02:58:25.000000 huhangkai-1.5.4/commen/__init__.py
+-rw-rw-rw-   0        0        0      543 2023-07-10 07:57:23.000000 huhangkai-1.5.4/commen/__main__.py
+drwxrwxrwx   0        0        0        0 2023-07-10 07:58:04.865267 huhangkai-1.5.4/commen/case_project/
+-rw-rw-rw-   0        0        0        0 2023-07-05 02:58:25.000000 huhangkai-1.5.4/commen/case_project/__init__.py
+-rw-rw-rw-   0        0        0     3080 2023-07-05 02:58:25.000000 huhangkai-1.5.4/commen/case_project/base_project.py
+-rw-rw-rw-   0        0        0      639 2023-07-05 09:37:54.000000 huhangkai-1.5.4/commen/case_project/json_coder.py
+-rw-rw-rw-   0        0        0      840 2023-07-10 06:49:07.000000 huhangkai-1.5.4/commen/case_project/setup_set.py
+-rw-rw-rw-   0        0        0       17 2023-07-10 07:58:04.000000 huhangkai-1.5.4/commen/case_project/version.py
+-rw-rw-rw-   0        0        0    29301 2023-07-10 06:34:54.000000 huhangkai-1.5.4/commen/init_project.py
+-rw-rw-rw-   0        0        0      276 2023-07-05 02:58:25.000000 huhangkai-1.5.4/commen/setup_run.py
+drwxrwxrwx   0        0        0        0 2023-07-10 07:58:04.867262 huhangkai-1.5.4/commen/testcase/
+-rw-rw-rw-   0        0        0        0 2023-07-05 02:58:25.000000 huhangkai-1.5.4/commen/testcase/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-10 07:58:04.909152 huhangkai-1.5.4/commen/testcase/apache/
+-rw-rw-rw-   0        0        0        0 2023-07-05 02:58:25.000000 huhangkai-1.5.4/commen/testcase/apache/__init__.py
+-rw-rw-rw-   0        0        0     3355 2023-07-05 02:58:25.000000 huhangkai-1.5.4/commen/testcase/apache/beam_class.py
+-rw-rw-rw-   0        0        0     5523 2023-07-05 02:58:25.000000 huhangkai-1.5.4/commen/testcase/apache/data.py
+-rw-rw-rw-   0        0        0     1764 2023-07-05 02:58:25.000000 huhangkai-1.5.4/commen/testcase/apache/par_do.py
+-rw-rw-rw-   0        0        0     7080 2023-07-05 02:58:25.000000 huhangkai-1.5.4/commen/testcase/apache/test_cogroupbykey.py
+-rw-rw-rw-   0        0        0      521 2023-07-05 08:50:31.000000 huhangkai-1.5.4/commen/testcase/apache/test_file.py
+-rw-rw-rw-   0        0        0     1548 2023-07-05 02:58:25.000000 huhangkai-1.5.4/commen/testcase/apache/test_fiter.py
+-rw-rw-rw-   0        0        0     2148 2023-07-05 02:58:25.000000 huhangkai-1.5.4/commen/testcase/apache/test_flatmap.py
+-rw-rw-rw-   0        0        0      568 2023-07-05 02:58:25.000000 huhangkai-1.5.4/commen/testcase/apache/test_map.py
+-rw-rw-rw-   0        0        0     2621 2023-07-05 02:58:25.000000 huhangkai-1.5.4/commen/testcase/apache/test_par_do.py
+-rw-rw-rw-   0        0        0     1696 2023-07-05 02:58:25.000000 huhangkai-1.5.4/commen/testcase/apache/test_regex.py
+-rw-rw-rw-   0        0        0      519 2023-07-05 02:58:25.000000 huhangkai-1.5.4/commen/testcase/apache/test_time.py
+-rw-rw-rw-   0        0        0      553 2023-07-05 02:58:25.000000 huhangkai-1.5.4/commen/testcase/apache/test_to_string.py
+-rw-rw-rw-   0        0        0    21837 2023-07-05 10:01:08.000000 huhangkai-1.5.4/commen/unit_apache_beam.py
+-rw-rw-rw-   0        0        0     4508 2023-07-05 02:58:25.000000 huhangkai-1.5.4/commen/unit_dict.py
+-rw-rw-rw-   0        0        0     3843 2023-07-05 02:58:25.000000 huhangkai-1.5.4/commen/unit_encryption.py
+-rw-rw-rw-   0        0        0    24880 2023-07-07 08:33:07.000000 huhangkai-1.5.4/commen/unit_fun.py
+-rw-rw-rw-   0        0        0     1242 2023-07-05 02:58:25.000000 huhangkai-1.5.4/commen/unit_logger.py
+-rw-rw-rw-   0        0        0     9218 2023-07-05 02:58:25.000000 huhangkai-1.5.4/commen/unit_request.py
+-rw-rw-rw-   0        0        0     2473 2023-07-05 02:58:25.000000 huhangkai-1.5.4/commen/unit_tasks.py
+-rw-rw-rw-   0        0        0      733 2023-07-05 02:58:25.000000 huhangkai-1.5.4/commen/常用命令.py
+drwxrwxrwx   0        0        0        0 2023-07-10 07:58:04.920122 huhangkai-1.5.4/huhangkai.egg-info/
+-rw-rw-rw-   0        0        0      228 2023-07-10 07:58:04.000000 huhangkai-1.5.4/huhangkai.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1107 2023-07-10 07:58:04.000000 huhangkai-1.5.4/huhangkai.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-10 07:58:04.000000 huhangkai-1.5.4/huhangkai.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      134 2023-07-10 07:58:04.000000 huhangkai-1.5.4/huhangkai.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-10 07:58:04.000000 huhangkai-1.5.4/huhangkai.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-10 07:58:04.923114 huhangkai-1.5.4/setup.cfg
+-rw-rw-rw-   0        0        0        2 2023-07-03 11:51:22.000000 huhangkai-1.5.4/setup.py
```

### Comparing `huhangkai-1.5.3/commen/__init__.py` & `huhangkai-1.5.4/commen/__init__.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.5.3/commen/case_project/base_project.py` & `huhangkai-1.5.4/commen/case_project/base_project.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.5.3/commen/case_project/json_coder.py` & `huhangkai-1.5.4/commen/case_project/json_coder.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.5.3/commen/case_project/setup_set.py` & `huhangkai-1.5.4/commen/case_project/setup_set.py`

 * *Files 13% similar despite different names*

```diff
@@ -24,11 +24,12 @@
         "pandas",
         "apache-beam",
         "pytest",
         "setuptools",
         "twine",
         "requests==2.29.0",
         "pandas",
+        "click",
     ],
 )
```

### Comparing `huhangkai-1.5.3/commen/init_project.py` & `huhangkai-1.5.4/commen/init_project.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -57,14 +57,24 @@
         # 获取已维护api方法接口列表
         self.get_api_fun_list()
         # 获取全量api接口列表
         self.get_api_list()
         # 添加api封装方法
         self.write_api_fun()
 
+    def set_file_path(self):
+        """创建项目目录"""
+        if not self.name:
+            self.name = os.path.basename(sys.argv[0])
+        self.service_dir = os.path.join(service_path, self.name)
+        self.testcase_dir = os.path.join(testcase_path, self.name)
+        FunBase.mkdir_file([self.service_dir, self.testcase_dir], is_py=False)
+        if not os.path.exists(os.path.join(self.service_dir, "__init__.py")):
+            FunBase.write_file(os.path.join(self.service_dir, "__init__.py"), value=self.get_init_value())
+
     def get_api_fun_list(self):
         """获取已维护方法列表，无则创建demo文件"""
         self.api_file_path = os.path.join(self.service_dir, self.name + "_api.py")
         if os.path.exists(self.api_file_path):
             self.api_file_str = FunBase.read_file(self.api_file_path)
         else:
             self.api_file_str = "import allure\n\nfrom service.%s import http_requester\n" \
@@ -131,24 +141,14 @@
             self.api_testcase_file_str = "import pytest\nimport allure\n\n" \
                                          "from service.%s.%s_api_fun import %sApiFun\n\n\n" % (
                                              self.name, self.name, self.name2)
             self.api_testcase_file_str += '@allure.epic("针对单api的测试")\n@allure.feature("场景：")\nclass TestApi:\n' \
                                           '    def setup(self):\n        self.f = %sApiFun()\n\n' % self.name2
         self.api_testcase_list = re.findall("    def +test_(.*)?\(", self.api_testcase_file_str)
 
-    def set_file_path(self):
-        """创建项目目录"""
-        if not self.name:
-            self.name = os.path.basename(sys.argv[0])
-        self.service_dir = os.path.join(service_path, self.name)
-        self.testcase_dir = os.path.join(testcase_path, self.name)
-        FunBase.mkdir_file([self.service_dir, self.testcase_dir], is_py=False)
-        if not os.path.exists(os.path.join(self.service_dir, "__init__.py")):
-            FunBase.write_file(os.path.join(self.service_dir, "__init__.py"), value=self.get_init_value())
-
     def get_api_list(self):
         """根据api文档不同方式生成api文件"""
         if self.api_type == 1:
             self.get_list_menu()
         elif self.api_type == 2:
             self.get_list_json()
         elif self.api_type == 0:
```

### Comparing `huhangkai-1.5.3/commen/testcase/apache/beam_class.py` & `huhangkai-1.5.4/commen/testcase/apache/beam_class.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.5.3/commen/testcase/apache/data.py` & `huhangkai-1.5.4/commen/testcase/apache/data.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.5.3/commen/testcase/apache/par_do.py` & `huhangkai-1.5.4/commen/testcase/apache/par_do.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.5.3/commen/testcase/apache/test_cogroupbykey.py` & `huhangkai-1.5.4/commen/testcase/apache/test_cogroupbykey.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.5.3/commen/testcase/apache/test_file.py` & `huhangkai-1.5.4/commen/testcase/apache/test_file.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.5.3/commen/testcase/apache/test_fiter.py` & `huhangkai-1.5.4/commen/testcase/apache/test_fiter.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.5.3/commen/testcase/apache/test_flatmap.py` & `huhangkai-1.5.4/commen/testcase/apache/test_flatmap.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.5.3/commen/testcase/apache/test_map.py` & `huhangkai-1.5.4/commen/testcase/apache/test_map.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.5.3/commen/testcase/apache/test_par_do.py` & `huhangkai-1.5.4/commen/testcase/apache/test_par_do.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.5.3/commen/testcase/apache/test_regex.py` & `huhangkai-1.5.4/commen/testcase/apache/test_regex.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.5.3/commen/testcase/apache/test_time.py` & `huhangkai-1.5.4/commen/testcase/apache/test_time.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.5.3/commen/testcase/apache/test_to_string.py` & `huhangkai-1.5.4/commen/testcase/apache/test_to_string.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.5.3/commen/unit_apache_beam.py` & `huhangkai-1.5.4/commen/unit_apache_beam.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.5.3/commen/unit_dict.py` & `huhangkai-1.5.4/commen/unit_dict.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.5.3/commen/unit_encryption.py` & `huhangkai-1.5.4/commen/unit_encryption.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.5.3/commen/unit_fun.py` & `huhangkai-1.5.4/commen/unit_fun.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.5.3/commen/unit_logger.py` & `huhangkai-1.5.4/commen/unit_logger.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.5.3/commen/unit_request.py` & `huhangkai-1.5.4/commen/unit_request.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.5.3/commen/unit_tasks.py` & `huhangkai-1.5.4/commen/unit_tasks.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.5.3/commen/常用命令.py` & `huhangkai-1.5.4/commen/常用命令.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.5.3/huhangkai.egg-info/SOURCES.txt` & `huhangkai-1.5.4/huhangkai.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 setup.py
 commen/__init__.py
+commen/__main__.py
 commen/init_project.py
 commen/setup_run.py
 commen/unit_apache_beam.py
 commen/unit_dict.py
 commen/unit_encryption.py
 commen/unit_fun.py
 commen/unit_logger.py
```

