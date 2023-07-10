# Comparing `tmp/huhangkai-1.5.4.tar.gz` & `tmp/huhangkai-1.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "huhangkai-1.5.4.tar", last modified: Mon Jul 10 07:58:04 2023, max compression
+gzip compressed data, was "huhangkai-1.5.5.tar", last modified: Mon Jul 10 08:28:31 2023, max compression
```

## Comparing `huhangkai-1.5.4.tar` & `huhangkai-1.5.5.tar`

### file list

```diff
@@ -1,45 +1,46 @@
-drwxrwxrwx   0        0        0        0 2023-07-10 07:58:04.923114 huhangkai-1.5.4/
--rw-rw-rw-   0        0        0      228 2023-07-10 07:58:04.922116 huhangkai-1.5.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-10 07:58:04.853299 huhangkai-1.5.4/commen/
--rw-rw-rw-   0        0        0      933 2023-07-05 02:58:25.000000 huhangkai-1.5.4/commen/__init__.py
--rw-rw-rw-   0        0        0      543 2023-07-10 07:57:23.000000 huhangkai-1.5.4/commen/__main__.py
-drwxrwxrwx   0        0        0        0 2023-07-10 07:58:04.865267 huhangkai-1.5.4/commen/case_project/
--rw-rw-rw-   0        0        0        0 2023-07-05 02:58:25.000000 huhangkai-1.5.4/commen/case_project/__init__.py
--rw-rw-rw-   0        0        0     3080 2023-07-05 02:58:25.000000 huhangkai-1.5.4/commen/case_project/base_project.py
--rw-rw-rw-   0        0        0      639 2023-07-05 09:37:54.000000 huhangkai-1.5.4/commen/case_project/json_coder.py
--rw-rw-rw-   0        0        0      840 2023-07-10 06:49:07.000000 huhangkai-1.5.4/commen/case_project/setup_set.py
--rw-rw-rw-   0        0        0       17 2023-07-10 07:58:04.000000 huhangkai-1.5.4/commen/case_project/version.py
--rw-rw-rw-   0        0        0    29301 2023-07-10 06:34:54.000000 huhangkai-1.5.4/commen/init_project.py
--rw-rw-rw-   0        0        0      276 2023-07-05 02:58:25.000000 huhangkai-1.5.4/commen/setup_run.py
-drwxrwxrwx   0        0        0        0 2023-07-10 07:58:04.867262 huhangkai-1.5.4/commen/testcase/
--rw-rw-rw-   0        0        0        0 2023-07-05 02:58:25.000000 huhangkai-1.5.4/commen/testcase/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-10 07:58:04.909152 huhangkai-1.5.4/commen/testcase/apache/
--rw-rw-rw-   0        0        0        0 2023-07-05 02:58:25.000000 huhangkai-1.5.4/commen/testcase/apache/__init__.py
--rw-rw-rw-   0        0        0     3355 2023-07-05 02:58:25.000000 huhangkai-1.5.4/commen/testcase/apache/beam_class.py
--rw-rw-rw-   0        0        0     5523 2023-07-05 02:58:25.000000 huhangkai-1.5.4/commen/testcase/apache/data.py
--rw-rw-rw-   0        0        0     1764 2023-07-05 02:58:25.000000 huhangkai-1.5.4/commen/testcase/apache/par_do.py
--rw-rw-rw-   0        0        0     7080 2023-07-05 02:58:25.000000 huhangkai-1.5.4/commen/testcase/apache/test_cogroupbykey.py
--rw-rw-rw-   0        0        0      521 2023-07-05 08:50:31.000000 huhangkai-1.5.4/commen/testcase/apache/test_file.py
--rw-rw-rw-   0        0        0     1548 2023-07-05 02:58:25.000000 huhangkai-1.5.4/commen/testcase/apache/test_fiter.py
--rw-rw-rw-   0        0        0     2148 2023-07-05 02:58:25.000000 huhangkai-1.5.4/commen/testcase/apache/test_flatmap.py
--rw-rw-rw-   0        0        0      568 2023-07-05 02:58:25.000000 huhangkai-1.5.4/commen/testcase/apache/test_map.py
--rw-rw-rw-   0        0        0     2621 2023-07-05 02:58:25.000000 huhangkai-1.5.4/commen/testcase/apache/test_par_do.py
--rw-rw-rw-   0        0        0     1696 2023-07-05 02:58:25.000000 huhangkai-1.5.4/commen/testcase/apache/test_regex.py
--rw-rw-rw-   0        0        0      519 2023-07-05 02:58:25.000000 huhangkai-1.5.4/commen/testcase/apache/test_time.py
--rw-rw-rw-   0        0        0      553 2023-07-05 02:58:25.000000 huhangkai-1.5.4/commen/testcase/apache/test_to_string.py
--rw-rw-rw-   0        0        0    21837 2023-07-05 10:01:08.000000 huhangkai-1.5.4/commen/unit_apache_beam.py
--rw-rw-rw-   0        0        0     4508 2023-07-05 02:58:25.000000 huhangkai-1.5.4/commen/unit_dict.py
--rw-rw-rw-   0        0        0     3843 2023-07-05 02:58:25.000000 huhangkai-1.5.4/commen/unit_encryption.py
--rw-rw-rw-   0        0        0    24880 2023-07-07 08:33:07.000000 huhangkai-1.5.4/commen/unit_fun.py
--rw-rw-rw-   0        0        0     1242 2023-07-05 02:58:25.000000 huhangkai-1.5.4/commen/unit_logger.py
--rw-rw-rw-   0        0        0     9218 2023-07-05 02:58:25.000000 huhangkai-1.5.4/commen/unit_request.py
--rw-rw-rw-   0        0        0     2473 2023-07-05 02:58:25.000000 huhangkai-1.5.4/commen/unit_tasks.py
--rw-rw-rw-   0        0        0      733 2023-07-05 02:58:25.000000 huhangkai-1.5.4/commen/常用命令.py
-drwxrwxrwx   0        0        0        0 2023-07-10 07:58:04.920122 huhangkai-1.5.4/huhangkai.egg-info/
--rw-rw-rw-   0        0        0      228 2023-07-10 07:58:04.000000 huhangkai-1.5.4/huhangkai.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1107 2023-07-10 07:58:04.000000 huhangkai-1.5.4/huhangkai.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-10 07:58:04.000000 huhangkai-1.5.4/huhangkai.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      134 2023-07-10 07:58:04.000000 huhangkai-1.5.4/huhangkai.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-10 07:58:04.000000 huhangkai-1.5.4/huhangkai.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-10 07:58:04.923114 huhangkai-1.5.4/setup.cfg
--rw-rw-rw-   0        0        0        2 2023-07-03 11:51:22.000000 huhangkai-1.5.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-10 08:28:31.817455 huhangkai-1.5.5/
+-rw-rw-rw-   0        0        0      228 2023-07-10 08:28:31.816460 huhangkai-1.5.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-10 08:28:31.749634 huhangkai-1.5.5/commen/
+-rw-rw-rw-   0        0        0      933 2023-07-05 02:58:25.000000 huhangkai-1.5.5/commen/__init__.py
+-rw-rw-rw-   0        0        0      543 2023-07-10 07:57:23.000000 huhangkai-1.5.5/commen/__main__.py
+drwxrwxrwx   0        0        0        0 2023-07-10 08:28:31.760606 huhangkai-1.5.5/commen/case_project/
+-rw-rw-rw-   0        0        0        0 2023-07-05 02:58:25.000000 huhangkai-1.5.5/commen/case_project/__init__.py
+-rw-rw-rw-   0        0        0     3080 2023-07-05 02:58:25.000000 huhangkai-1.5.5/commen/case_project/base_project.py
+-rw-rw-rw-   0        0        0      639 2023-07-05 09:37:54.000000 huhangkai-1.5.5/commen/case_project/json_coder.py
+-rw-rw-rw-   0        0        0      946 2023-07-10 08:28:10.000000 huhangkai-1.5.5/commen/case_project/setup_set.py
+-rw-rw-rw-   0        0        0       17 2023-07-10 08:28:31.000000 huhangkai-1.5.5/commen/case_project/version.py
+-rw-rw-rw-   0        0        0    29339 2023-07-10 08:27:36.000000 huhangkai-1.5.5/commen/init_project.py
+-rw-rw-rw-   0        0        0      276 2023-07-05 02:58:25.000000 huhangkai-1.5.5/commen/setup_run.py
+drwxrwxrwx   0        0        0        0 2023-07-10 08:28:31.762599 huhangkai-1.5.5/commen/testcase/
+-rw-rw-rw-   0        0        0        0 2023-07-05 02:58:25.000000 huhangkai-1.5.5/commen/testcase/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-10 08:28:31.800498 huhangkai-1.5.5/commen/testcase/apache/
+-rw-rw-rw-   0        0        0        0 2023-07-05 02:58:25.000000 huhangkai-1.5.5/commen/testcase/apache/__init__.py
+-rw-rw-rw-   0        0        0     3355 2023-07-05 02:58:25.000000 huhangkai-1.5.5/commen/testcase/apache/beam_class.py
+-rw-rw-rw-   0        0        0     5523 2023-07-05 02:58:25.000000 huhangkai-1.5.5/commen/testcase/apache/data.py
+-rw-rw-rw-   0        0        0     1764 2023-07-05 02:58:25.000000 huhangkai-1.5.5/commen/testcase/apache/par_do.py
+-rw-rw-rw-   0        0        0     7080 2023-07-05 02:58:25.000000 huhangkai-1.5.5/commen/testcase/apache/test_cogroupbykey.py
+-rw-rw-rw-   0        0        0      521 2023-07-05 08:50:31.000000 huhangkai-1.5.5/commen/testcase/apache/test_file.py
+-rw-rw-rw-   0        0        0     1548 2023-07-05 02:58:25.000000 huhangkai-1.5.5/commen/testcase/apache/test_fiter.py
+-rw-rw-rw-   0        0        0     2148 2023-07-05 02:58:25.000000 huhangkai-1.5.5/commen/testcase/apache/test_flatmap.py
+-rw-rw-rw-   0        0        0      568 2023-07-05 02:58:25.000000 huhangkai-1.5.5/commen/testcase/apache/test_map.py
+-rw-rw-rw-   0        0        0     2621 2023-07-05 02:58:25.000000 huhangkai-1.5.5/commen/testcase/apache/test_par_do.py
+-rw-rw-rw-   0        0        0     1696 2023-07-05 02:58:25.000000 huhangkai-1.5.5/commen/testcase/apache/test_regex.py
+-rw-rw-rw-   0        0        0      519 2023-07-05 02:58:25.000000 huhangkai-1.5.5/commen/testcase/apache/test_time.py
+-rw-rw-rw-   0        0        0      553 2023-07-05 02:58:25.000000 huhangkai-1.5.5/commen/testcase/apache/test_to_string.py
+-rw-rw-rw-   0        0        0    21837 2023-07-05 10:01:08.000000 huhangkai-1.5.5/commen/unit_apache_beam.py
+-rw-rw-rw-   0        0        0     4508 2023-07-05 02:58:25.000000 huhangkai-1.5.5/commen/unit_dict.py
+-rw-rw-rw-   0        0        0     3843 2023-07-05 02:58:25.000000 huhangkai-1.5.5/commen/unit_encryption.py
+-rw-rw-rw-   0        0        0    24880 2023-07-07 08:33:07.000000 huhangkai-1.5.5/commen/unit_fun.py
+-rw-rw-rw-   0        0        0     1242 2023-07-05 02:58:25.000000 huhangkai-1.5.5/commen/unit_logger.py
+-rw-rw-rw-   0        0        0     9218 2023-07-05 02:58:25.000000 huhangkai-1.5.5/commen/unit_request.py
+-rw-rw-rw-   0        0        0     2473 2023-07-05 02:58:25.000000 huhangkai-1.5.5/commen/unit_tasks.py
+-rw-rw-rw-   0        0        0      733 2023-07-05 02:58:25.000000 huhangkai-1.5.5/commen/常用命令.py
+drwxrwxrwx   0        0        0        0 2023-07-10 08:28:31.814463 huhangkai-1.5.5/huhangkai.egg-info/
+-rw-rw-rw-   0        0        0      228 2023-07-10 08:28:31.000000 huhangkai-1.5.5/huhangkai.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1143 2023-07-10 08:28:31.000000 huhangkai-1.5.5/huhangkai.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-10 08:28:31.000000 huhangkai-1.5.5/huhangkai.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       82 2023-07-10 08:28:31.000000 huhangkai-1.5.5/huhangkai.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      134 2023-07-10 08:28:31.000000 huhangkai-1.5.5/huhangkai.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-10 08:28:31.000000 huhangkai-1.5.5/huhangkai.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-10 08:28:31.817455 huhangkai-1.5.5/setup.cfg
+-rw-rw-rw-   0        0        0        2 2023-07-03 11:51:22.000000 huhangkai-1.5.5/setup.py
```

### Comparing `huhangkai-1.5.4/commen/__init__.py` & `huhangkai-1.5.5/commen/__init__.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.5.4/commen/__main__.py` & `huhangkai-1.5.5/commen/__main__.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.5.4/commen/case_project/base_project.py` & `huhangkai-1.5.5/commen/case_project/base_project.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.5.4/commen/case_project/json_coder.py` & `huhangkai-1.5.5/commen/case_project/json_coder.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.5.4/commen/case_project/setup_set.py` & `huhangkai-1.5.5/commen/case_project/setup_set.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,14 +8,15 @@
     description='接口自动化',  # 描述
     author='胡杭凯',  # 作者
     author_email='3173825608@qq.com',
     # package_dir={"": "commen"},
     packages=find_packages(),
     package_data={'by': ['常用命令.py'],},
     include_package_data=True,
+    entry_points={'console_scripts': ['hhk=commen.init_project:main', 'init=commen.init_project:main']},
     python_requires=">=3.0",
     install_requires=[
         "faker",
         "openpyxl",
         "apscheduler",
         "rsa",
         "pyDes",
```

### Comparing `huhangkai-1.5.4/commen/init_project.py` & `huhangkai-1.5.5/commen/init_project.py`

 * *Files 0% similar despite different names*

```diff
@@ -538,10 +538,12 @@
                     _str = _str.replace(name, desc)
         if re.findall(r'[( ]async[,=)]', _str):
             for tmp in re.findall(r'[( ]async[,=)]', _str):
                 tmp1 = str(tmp).replace('async', 'async1')
                 _str = _str.replace(tmp, tmp1)
         return _str
 
+def main():
+    print("hello world!")
 
 if __name__ == '__main__':
     GetApi(app_key="a63ca17b-3cf3-46cb-b8b6-9ad20518e1e1")
```

### Comparing `huhangkai-1.5.4/commen/testcase/apache/beam_class.py` & `huhangkai-1.5.5/commen/testcase/apache/beam_class.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.5.4/commen/testcase/apache/data.py` & `huhangkai-1.5.5/commen/testcase/apache/data.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.5.4/commen/testcase/apache/par_do.py` & `huhangkai-1.5.5/commen/testcase/apache/par_do.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.5.4/commen/testcase/apache/test_cogroupbykey.py` & `huhangkai-1.5.5/commen/testcase/apache/test_cogroupbykey.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.5.4/commen/testcase/apache/test_file.py` & `huhangkai-1.5.5/commen/testcase/apache/test_file.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.5.4/commen/testcase/apache/test_fiter.py` & `huhangkai-1.5.5/commen/testcase/apache/test_fiter.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.5.4/commen/testcase/apache/test_flatmap.py` & `huhangkai-1.5.5/commen/testcase/apache/test_flatmap.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.5.4/commen/testcase/apache/test_map.py` & `huhangkai-1.5.5/commen/testcase/apache/test_map.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.5.4/commen/testcase/apache/test_par_do.py` & `huhangkai-1.5.5/commen/testcase/apache/test_par_do.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.5.4/commen/testcase/apache/test_regex.py` & `huhangkai-1.5.5/commen/testcase/apache/test_regex.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.5.4/commen/testcase/apache/test_time.py` & `huhangkai-1.5.5/commen/testcase/apache/test_time.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.5.4/commen/testcase/apache/test_to_string.py` & `huhangkai-1.5.5/commen/testcase/apache/test_to_string.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.5.4/commen/unit_apache_beam.py` & `huhangkai-1.5.5/commen/unit_apache_beam.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.5.4/commen/unit_dict.py` & `huhangkai-1.5.5/commen/unit_dict.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.5.4/commen/unit_encryption.py` & `huhangkai-1.5.5/commen/unit_encryption.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.5.4/commen/unit_fun.py` & `huhangkai-1.5.5/commen/unit_fun.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.5.4/commen/unit_logger.py` & `huhangkai-1.5.5/commen/unit_logger.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.5.4/commen/unit_request.py` & `huhangkai-1.5.5/commen/unit_request.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.5.4/commen/unit_tasks.py` & `huhangkai-1.5.5/commen/unit_tasks.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.5.4/commen/常用命令.py` & `huhangkai-1.5.5/commen/常用命令.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.5.4/huhangkai.egg-info/SOURCES.txt` & `huhangkai-1.5.5/huhangkai.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -29,9 +29,10 @@
 commen/testcase/apache/test_par_do.py
 commen/testcase/apache/test_regex.py
 commen/testcase/apache/test_time.py
 commen/testcase/apache/test_to_string.py
 huhangkai.egg-info/PKG-INFO
 huhangkai.egg-info/SOURCES.txt
 huhangkai.egg-info/dependency_links.txt
+huhangkai.egg-info/entry_points.txt
 huhangkai.egg-info/requires.txt
 huhangkai.egg-info/top_level.txt
```

