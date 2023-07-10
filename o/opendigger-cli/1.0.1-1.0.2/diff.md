# Comparing `tmp/opendigger_cli-1.0.1-py3-none-any.whl.zip` & `tmp/opendigger_cli-1.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 5318 bytes, number of entries: 7
+Zip file size: 5334 bytes, number of entries: 7
 -rw-r--r--  2.0 unx        0 b- defN 23-Jun-28 13:26 opendigger-cli/__init__.py
 -rw-r--r--  2.0 unx     1006 b- defN 23-Jul-08 10:16 opendigger-cli/__main__.py
--rw-r--r--  2.0 unx    14963 b- defN 23-Jul-08 10:16 opendigger-cli/func.py
--rw-r--r--  2.0 unx      229 b- defN 23-Jul-08 10:18 opendigger_cli-1.0.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-08 10:18 opendigger_cli-1.0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       15 b- defN 23-Jul-08 10:18 opendigger_cli-1.0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      568 b- defN 23-Jul-08 10:18 opendigger_cli-1.0.1.dist-info/RECORD
-7 files, 16873 bytes uncompressed, 4304 bytes compressed:  74.5%
+-rw-r--r--  2.0 unx    15184 b- defN 23-Jul-10 14:39 opendigger-cli/func.py
+-rw-r--r--  2.0 unx      229 b- defN 23-Jul-10 14:39 opendigger_cli-1.0.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-10 14:39 opendigger_cli-1.0.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       15 b- defN 23-Jul-10 14:39 opendigger_cli-1.0.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      568 b- defN 23-Jul-10 14:39 opendigger_cli-1.0.2.dist-info/RECORD
+7 files, 17094 bytes uncompressed, 4320 bytes compressed:  74.7%
```

## zipnote {}

```diff
@@ -3,20 +3,20 @@
 
 Filename: opendigger-cli/__main__.py
 Comment: 
 
 Filename: opendigger-cli/func.py
 Comment: 
 
-Filename: opendigger_cli-1.0.1.dist-info/METADATA
+Filename: opendigger_cli-1.0.2.dist-info/METADATA
 Comment: 
 
-Filename: opendigger_cli-1.0.1.dist-info/WHEEL
+Filename: opendigger_cli-1.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: opendigger_cli-1.0.1.dist-info/top_level.txt
+Filename: opendigger_cli-1.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: opendigger_cli-1.0.1.dist-info/RECORD
+Filename: opendigger_cli-1.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## opendigger-cli/func.py

```diff
@@ -229,54 +229,61 @@
         plt.suptitle(name)
         if path is not None:
             save_path = path
         else:
             save_path = "./picture.jpg"
         plt.savefig(save_path)
 
-    def print_result(self, args):
-        """
-        以json格式输出结果至控制台
-        :param args:
-        :return:
-        """
-        repo_name = args.repo.split('/')[-1]
-        print(f'repo name: {repo_name}')
-        print(f'repo url: https://github.com/{args.repo}')
-        result_json = json.dumps(self.result_dict)
-        print(result_json)
+    def print_result(self, option):
+        if '/' in option:
+            print(f'repo name: {option}')
+            print(f'repo url: https://github.com/{option}')
+        else:
+            print(f'user name: {option}')
+            print(f'user url: https://github.com/{option}')
 
-    def output_pdf(self, args, metric_list):
+        print()
+
+        for key, value in self.result_dict.items():
+            print(key)
+            print(value)
+
+    def output_pdf(self, args, option, metric_list):
         """
         将结果输出至PDF中
         :param args:
         :param metric_list:
         :return:
         """
         save_path = args.save_path
         output_path_pdf = f'{save_path}report.pdf' if save_path[-1] == '/' else f'{save_path}/report.pdf'
 
         pdf = fpdf.FPDF(format='letter', unit='in')
         pdf.add_page()
         pdf.set_font('Times', '', 13)
         pdf.set_line_width(0.5)
         effective_page_width = pdf.w - 2*pdf.l_margin
-        repo_name = args.repo.split('/')[-1]
+
         result_json = json.dumps(self.result_dict)
-        pdf.multi_cell(effective_page_width, 0.3, f'repo name: {repo_name}')
-        pdf.multi_cell(effective_page_width, 0.3, f'repo url: https://github.com/{args.repo}')
+        if '/' in option:
+            pdf.multi_cell(effective_page_width, 0.3, f'repo name: {option}')
+            pdf.multi_cell(effective_page_width, 0.3, f'repo url: https://github.com/{option}')
+        else:
+            pdf.multi_cell(effective_page_width, 0.3, f'user name: {option}')
+            pdf.multi_cell(effective_page_width, 0.3, f'user url: https://github.com/{option}')
+
         pdf.multi_cell(effective_page_width, 0.3, result_json)
 
         jpg_list = list()
         for i, res in enumerate(self.response_contents):
             can_print = OpenDiggerCLI.get_pic_json(metric_list[i])
             if can_print is False:
                 continue
             output_path_jpg = f'{save_path}picture{i}.jpg' if save_path[-1] == '/' else f'{save_path}/picture{i}.jpg'
-            OpenDiggerCLI.print_pic(f'{metric_list[i]} for {args.repo}', 'time', metric_list[i], res, output_path_jpg)
+            OpenDiggerCLI.print_pic(f'{metric_list[i]} for {option}', 'time', metric_list[i], res, output_path_jpg)
             jpg_list.append(output_path_jpg)
             pdf.image(output_path_jpg, w=6, h=4.5)
         pdf.output(output_path_pdf, 'F')
 
         for item in jpg_list:
             os.remove(item)
 
@@ -346,15 +353,15 @@
         self.query_network(metric_list=network_metric_list, node_list=node_list, edge_list=edge_list,
                            option=option)
 
         # debug
         # print(query_result_dict)
 
         if download:
-            output_path = self.output_pdf(args, temp_metric_list)
+            output_path = self.output_pdf(args, option, temp_metric_list)
             print('[INFO] the pdf output is completed and saved at ', output_path)
         else:
-            self.print_result(args)
+            self.print_result(option)
```

## Comparing `opendigger_cli-1.0.1.dist-info/RECORD` & `opendigger_cli-1.0.2.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 opendigger-cli/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 opendigger-cli/__main__.py,sha256=kZNWYea_EedT9czFdNbsCYOG3IU62vSWyhFs7Elk9h8,1006
-opendigger-cli/func.py,sha256=TgSwbqOxaD-iop2V0IbEBCV7V6Wm9wELfZx7r6kcO0w,14963
-opendigger_cli-1.0.1.dist-info/METADATA,sha256=632jmpulCSenGVdf-TGJ2nHoRAOb1suk90KCarm4AVo,229
-opendigger_cli-1.0.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-opendigger_cli-1.0.1.dist-info/top_level.txt,sha256=M4vrOJ6iIAsdxRlbPnX7V8oAf_mVwsLv8OGbj8dVq8c,15
-opendigger_cli-1.0.1.dist-info/RECORD,,
+opendigger-cli/func.py,sha256=0hnmKo0KnwOveMVGgYN6MaFkQPbpHWckqad0KqFrIsA,15184
+opendigger_cli-1.0.2.dist-info/METADATA,sha256=5dM7LdwQ5cnr5x71q9iq-XJaQgyW7wweO7-0aXWeL6U,229
+opendigger_cli-1.0.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+opendigger_cli-1.0.2.dist-info/top_level.txt,sha256=M4vrOJ6iIAsdxRlbPnX7V8oAf_mVwsLv8OGbj8dVq8c,15
+opendigger_cli-1.0.2.dist-info/RECORD,,
```

