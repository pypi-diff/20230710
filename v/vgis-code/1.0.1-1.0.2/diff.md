# Comparing `tmp/vgis_code-1.0.1.tar.gz` & `tmp/vgis_code-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\vgis_code-1.0.1.tar", last modified: Fri Jul  7 10:27:41 2023, max compression
+gzip compressed data, was "dist\vgis_code-1.0.2.tar", last modified: Mon Jul 10 07:25:24 2023, max compression
```

## Comparing `vgis_code-1.0.1.tar` & `vgis_code-1.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-07 10:27:41.485383 vgis_code-1.0.1/
--rw-rw-rw-   0        0        0     1061 2023-07-07 10:27:41.475383 vgis_code-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      128 2023-07-07 09:39:22.000000 vgis_code-1.0.1/README.md
--rw-rw-rw-   0        0        0       42 2023-07-07 10:27:41.486383 vgis_code-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     2202 2023-07-07 09:40:47.000000 vgis_code-1.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-07 10:27:41.465382 vgis_code-1.0.1/vgis_code/
--rw-rw-rw-   0        0        0      202 2023-06-27 07:23:55.000000 vgis_code-1.0.1/vgis_code/__init__.py
--rw-rw-rw-   0        0        0    53633 2023-07-07 10:25:43.000000 vgis_code-1.0.1/vgis_code/codeGenerator.py
-drwxrwxrwx   0        0        0        0 2023-07-07 10:27:41.473383 vgis_code-1.0.1/vgis_code.egg-info/
--rw-rw-rw-   0        0        0     1061 2023-07-07 10:27:41.000000 vgis_code-1.0.1/vgis_code.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      231 2023-07-07 10:27:41.000000 vgis_code-1.0.1/vgis_code.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-07 10:27:41.000000 vgis_code-1.0.1/vgis_code.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2023-07-07 10:27:41.000000 vgis_code-1.0.1/vgis_code.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-07 10:27:41.000000 vgis_code-1.0.1/vgis_code.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-10 07:25:24.606760 vgis_code-1.0.2/
+-rw-rw-rw-   0        0        0     1061 2023-07-10 07:25:24.605760 vgis_code-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      128 2023-07-07 09:39:22.000000 vgis_code-1.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-10 07:25:24.606760 vgis_code-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     2202 2023-07-10 07:25:04.000000 vgis_code-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-10 07:25:24.595760 vgis_code-1.0.2/vgis_code/
+-rw-rw-rw-   0        0        0      202 2023-06-27 07:23:55.000000 vgis_code-1.0.2/vgis_code/__init__.py
+-rw-rw-rw-   0        0        0    54033 2023-07-10 07:23:53.000000 vgis_code-1.0.2/vgis_code/codeGenerator.py
+drwxrwxrwx   0        0        0        0 2023-07-10 07:25:24.604760 vgis_code-1.0.2/vgis_code.egg-info/
+-rw-rw-rw-   0        0        0     1061 2023-07-10 07:25:24.000000 vgis_code-1.0.2/vgis_code.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      231 2023-07-10 07:25:24.000000 vgis_code-1.0.2/vgis_code.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-10 07:25:24.000000 vgis_code-1.0.2/vgis_code.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-07-10 07:25:24.000000 vgis_code-1.0.2/vgis_code.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-10 07:25:24.000000 vgis_code-1.0.2/vgis_code.egg-info/top_level.txt
```

### Comparing `vgis_code-1.0.1/PKG-INFO` & `vgis_code-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vgis_code
-Version: 1.0.1
+Version: 1.0.2
 Summary: A libary for code generator operator
 Home-page: https://github.com/gisfanmachel/vgisDatabase
 Author: gisfanmachel
 Author-email: gisfanmachel@gmail.com
 License: UNKNOWN
 Description: ## this  is  vgis code generator lib
```

### Comparing `vgis_code-1.0.1/setup.py` & `vgis_code-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 # Arguments marked as "Required" below must be included for upload to PyPI.
 # Fields marked as "Optional" may be commented out.
 
 setup(
 
     name="vgis_code",  # Required 项目名称
-    version="1.0.1",  # Required 发布版本号
+    version="1.0.2",  # Required 发布版本号
     description="A libary for code generator operator",  # Optional 项目简单描述
     long_description=long_description,  # Optional 详细描述
     long_description_content_type="text/markdown",  # 内容类型
     url="https://github.com/gisfanmachel/vgisDatabase",  # Optional github项目地址
     author="gisfanmachel",  # Optional 作者
     author_email="gisfanmachel@gmail.com",  # Optional 作者邮箱
     classifiers=[  # Optional 分类器通过对项目进行分类来帮助用户找到项目, 以下除了python版本其他的 不需要改动
```

### Comparing `vgis_code-1.0.1/vgis_code/codeGenerator.py` & `vgis_code-1.0.2/vgis_code/codeGenerator.py`

 * *Files 2% similar despite different names*

```diff
@@ -178,14 +178,15 @@
             if row % 3 == 0:
                 line = line.strip('\n')
                 line2 = self.decapitalize(line)
                 print("router.register(r'{}', {}ViewSet, basename='{}')".format(line2, line, line2))
             row = row + 1
 
     # 生成postman测试用例
+    # 基于已有的基础用例添加业务用例
     def generate_postman(self):
         # postman_json = {}
         #
         # # 读取json文件
         # with open(self.postmanFile, 'r', encoding="UTF-8") as f:
         #     postman_json = json.load(f)
 
@@ -206,20 +207,23 @@
             line = file.readline().strip('\n')
             count_index = 0
             table_index = 0
             while line:
                 # 判断是否为表的开始
                 if int(count_index / 3) == table_index:
                     # 指定表的第一行，表类名
+                    # TtInsuranceProjectMilestone
                     if count_index % 3 == 0:
                         tableClass = line
                     # 指定表的第二行，表英文名
+                    # tt_insurance_project_milestone
                     if count_index % 3 == 1:
                         tableEname = line
                     # 指定表的第三行，表中文名
+                    # 保险项目里程碑
                     if count_index % 3 == 2:
                         tableCname = line
                         table_index += 1
                         sub_item_obj = {}
                         sub_item_obj["name"] = tableCname
                         single_item_list = []
 
@@ -261,21 +265,21 @@
                                 "options": {
                                     "raw": {
                                         "language": "json"
                                     }
                                 }
                             },
                             "url": {
-                                "raw": "{{service_host}}/{}/{}".format(self.apiPath, tableClass),
+                                "raw": "{{service_host}}/{}/{}".format(self.apiPath, self.decapitalize(tableClass)),
                                 "host": [
                                     "{{service_host}}"
                                 ],
                                 "path": [
                                     "{}".format(self.apiPath),
-                                    "{}".format(tableClass)
+                                    "{}".format(self.decapitalize(tableClass))
                                 ]
                             }
                         }
                         single_item_obj["response"] = []
                         single_item_list.append(single_item_obj)
 
                         # 新增接口
@@ -315,21 +319,21 @@
                                 "options": {
                                     "raw": {
                                         "language": "json"
                                     }
                                 }
                             },
                             "url": {
-                                "raw": "{{service_host}}/{}/{}/".format(self.apiPath, tableClass),
+                                "raw": "{{service_host}}/{}/{}/".format(self.apiPath, self.decapitalize(tableClass)),
                                 "host": [
                                     "{{service_host}}"
                                 ],
                                 "path": [
                                     "{}".format(self.apiPath),
-                                    "{}".format(tableClass),
+                                    "{}".format(self.decapitalize(tableClass)),
                                     ""
                                 ]
                             }
                         }
                         single_item_obj["response"] = []
                         single_item_list.append(single_item_obj)
 
@@ -370,21 +374,21 @@
                                 "options": {
                                     "raw": {
                                         "language": "json"
                                     }
                                 }
                             },
                             "url": {
-                                "raw": "{{service_host}}/{}/{}/17/".format(self.apiPath, tableClass),
+                                "raw": "{{service_host}}/{}/{}/17/".format(self.apiPath, self.decapitalize(tableClass)),
                                 "host": [
                                     "{{service_host}}"
                                 ],
                                 "path": [
                                     "{}".format(self.apiPath),
-                                    "{}".format(tableClass),
+                                    "{}".format(self.decapitalize(tableClass)),
                                     "17",
                                     ""
                                 ]
                             }
                         }
                         single_item_obj["response"] = []
                         single_item_list.append(single_item_obj)
@@ -427,21 +431,21 @@
                                 "options": {
                                     "raw": {
                                         "language": "json"
                                     }
                                 }
                             },
                             "url": {
-                                "raw": "{{service_host}}/{}/{}/17/".format(self.apiPath, tableClass),
+                                "raw": "{{service_host}}/{}/{}/17/".format(self.apiPath, self.decapitalize(tableClass)),
                                 "host": [
                                     "{{service_host}}"
                                 ],
                                 "path": [
                                     "{}".format(self.apiPath),
-                                    "{}".format(tableClass),
+                                    "{}".format(self.decapitalize(tableClass)),
                                     "17",
                                     ""
                                 ]
                             }
                         }
                         single_item_obj["response"] = []
                         single_item_list.append(single_item_obj)
@@ -483,21 +487,21 @@
                                 "options": {
                                     "raw": {
                                         "language": "json"
                                     }
                                 }
                             },
                             "url": {
-                                "raw": "{{service_host}}/{}/{}/26/".format(self.apiPath, tableClass),
+                                "raw": "{{service_host}}/{}/{}/26/".format(self.apiPath, self.decapitalize(tableClass)),
                                 "host": [
                                     "{{service_host}}"
                                 ],
                                 "path": [
                                     "{}".format(self.apiPath),
-                                    "{}".format(tableClass),
+                                    "{}".format(self.decapitalize(tableClass)),
                                     "26",
                                     ""
                                 ]
                             }
                         }
                         single_item_obj["response"] = []
                         single_item_list.append(single_item_obj)
@@ -898,15 +902,15 @@
 #     # 需要判断是否连接可视化数据库成功
 #     return conn
 
 
 # 生成django代码
 def make_django_code():
     model_file = "E:\\model.txt"
-    api_path = "api"
+    api_path = "wxgzgl_api"
     host = "192.168.3.191"
     port = "5432"
     user = "postgres"
     passwd = "postgres123"
     database = "BXJCXTDB"
     connection = PgHelper.get_database_conection(host, port, user, passwd, database)
     postman_file = "E:\\通用项目.postman_collection.json"
```

### Comparing `vgis_code-1.0.1/vgis_code.egg-info/PKG-INFO` & `vgis_code-1.0.2/vgis_code.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vgis-code
-Version: 1.0.1
+Version: 1.0.2
 Summary: A libary for code generator operator
 Home-page: https://github.com/gisfanmachel/vgisDatabase
 Author: gisfanmachel
 Author-email: gisfanmachel@gmail.com
 License: UNKNOWN
 Description: ## this  is  vgis code generator lib
```

