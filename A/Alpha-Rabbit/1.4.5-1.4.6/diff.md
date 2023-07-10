# Comparing `tmp/Alpha_Rabbit-1.4.5.tar.gz` & `tmp/Alpha_Rabbit-1.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Alpha_Rabbit-1.4.5.tar", last modified: Mon Jul 10 08:17:26 2023, max compression
+gzip compressed data, was "Alpha_Rabbit-1.4.6.tar", last modified: Mon Jul 10 10:04:14 2023, max compression
```

## Comparing `Alpha_Rabbit-1.4.5.tar` & `Alpha_Rabbit-1.4.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-07-10 08:17:26.027681 Alpha_Rabbit-1.4.5/
-drwxrwxrwx   0        0        0        0 2023-07-10 08:17:26.019159 Alpha_Rabbit-1.4.5/Alpha_Rabbit/
--rw-rw-rw-   0        0        0    42376 2023-07-10 08:14:29.000000 Alpha_Rabbit-1.4.5/Alpha_Rabbit/Alpha_Rabbit.py
--rw-rw-rw-   0        0        0    13979 2023-07-10 08:16:58.000000 Alpha_Rabbit-1.4.5/Alpha_Rabbit/Factor_Calculator.py
--rw-rw-rw-   0        0        0    22658 2023-06-05 07:41:31.000000 Alpha_Rabbit-1.4.5/Alpha_Rabbit/Factor_Def_and_Get_Method.py
--rw-rw-rw-   0        0        0        0 2023-02-27 02:16:19.000000 Alpha_Rabbit-1.4.5/Alpha_Rabbit/__init__.py
--rw-rw-rw-   0        0        0     1522 2023-02-27 02:16:19.000000 Alpha_Rabbit-1.4.5/Alpha_Rabbit/trade_strategy.py
-drwxrwxrwx   0        0        0        0 2023-07-10 08:17:26.026324 Alpha_Rabbit-1.4.5/Alpha_Rabbit.egg-info/
--rw-rw-rw-   0        0        0      787 2023-07-10 08:17:25.000000 Alpha_Rabbit-1.4.5/Alpha_Rabbit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      411 2023-07-10 08:17:25.000000 Alpha_Rabbit-1.4.5/Alpha_Rabbit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-10 08:17:25.000000 Alpha_Rabbit-1.4.5/Alpha_Rabbit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-07-10 08:17:25.000000 Alpha_Rabbit-1.4.5/Alpha_Rabbit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-07-10 08:17:25.000000 Alpha_Rabbit-1.4.5/Alpha_Rabbit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-02-27 02:16:19.000000 Alpha_Rabbit-1.4.5/Alpha_Rabbit.egg-info/zip-safe
--rw-rw-rw-   0        0        0     1094 2023-02-27 02:16:19.000000 Alpha_Rabbit-1.4.5/LICENSE.txt
--rw-rw-rw-   0        0        0      787 2023-07-10 08:17:26.027681 Alpha_Rabbit-1.4.5/PKG-INFO
--rw-rw-rw-   0        0        0       69 2023-02-27 02:16:19.000000 Alpha_Rabbit-1.4.5/README.md
--rw-rw-rw-   0        0        0       85 2023-07-10 08:17:26.028727 Alpha_Rabbit-1.4.5/setup.cfg
--rw-rw-rw-   0        0        0     1229 2023-07-10 08:17:12.000000 Alpha_Rabbit-1.4.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-10 10:04:14.193369 Alpha_Rabbit-1.4.6/
+drwxrwxrwx   0        0        0        0 2023-07-10 10:04:13.916326 Alpha_Rabbit-1.4.6/Alpha_Rabbit/
+-rw-rw-rw-   0        0        0    42540 2023-07-10 10:03:27.000000 Alpha_Rabbit-1.4.6/Alpha_Rabbit/Alpha_Rabbit.py
+-rw-rw-rw-   0        0        0    13979 2023-07-10 08:16:58.000000 Alpha_Rabbit-1.4.6/Alpha_Rabbit/Factor_Calculator.py
+-rw-rw-rw-   0        0        0    22658 2023-06-05 07:41:31.000000 Alpha_Rabbit-1.4.6/Alpha_Rabbit/Factor_Def_and_Get_Method.py
+-rw-rw-rw-   0        0        0        0 2023-02-27 02:16:19.000000 Alpha_Rabbit-1.4.6/Alpha_Rabbit/__init__.py
+-rw-rw-rw-   0        0        0     1522 2023-02-27 02:16:19.000000 Alpha_Rabbit-1.4.6/Alpha_Rabbit/trade_strategy.py
+drwxrwxrwx   0        0        0        0 2023-07-10 10:04:13.984567 Alpha_Rabbit-1.4.6/Alpha_Rabbit.egg-info/
+-rw-rw-rw-   0        0        0      787 2023-07-10 10:04:13.000000 Alpha_Rabbit-1.4.6/Alpha_Rabbit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      411 2023-07-10 10:04:13.000000 Alpha_Rabbit-1.4.6/Alpha_Rabbit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-10 10:04:13.000000 Alpha_Rabbit-1.4.6/Alpha_Rabbit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-07-10 10:04:13.000000 Alpha_Rabbit-1.4.6/Alpha_Rabbit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-07-10 10:04:13.000000 Alpha_Rabbit-1.4.6/Alpha_Rabbit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-02-27 02:16:19.000000 Alpha_Rabbit-1.4.6/Alpha_Rabbit.egg-info/zip-safe
+-rw-rw-rw-   0        0        0     1094 2023-02-27 02:16:19.000000 Alpha_Rabbit-1.4.6/LICENSE.txt
+-rw-rw-rw-   0        0        0      787 2023-07-10 10:04:14.193369 Alpha_Rabbit-1.4.6/PKG-INFO
+-rw-rw-rw-   0        0        0       69 2023-02-27 02:16:19.000000 Alpha_Rabbit-1.4.6/README.md
+-rw-rw-rw-   0        0        0       85 2023-07-10 10:04:14.196368 Alpha_Rabbit-1.4.6/setup.cfg
+-rw-rw-rw-   0        0        0     1229 2023-07-10 10:03:58.000000 Alpha_Rabbit-1.4.6/setup.py
```

### Comparing `Alpha_Rabbit-1.4.5/Alpha_Rabbit/Alpha_Rabbit.py` & `Alpha_Rabbit-1.4.6/Alpha_Rabbit/Alpha_Rabbit.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,15 +83,19 @@
                               Price,
                               days,
                               savedir,
                               demean = False):
         from alphalens import utils
         plottools = plot_tools()
         mate_al = mate_alphalens()
-        to = res_df.groupby(by = fcname+'_quantile').apply(lambda x: self.cal_turnover(x[fcname+'_quantile']/x[fcname+'_quantile'],days)).mean(axis =1)
+        tov_df = res_df.groupby(by = fcname+'_quantile').apply(lambda x: self.cal_turnover(x[fcname+'_quantile']/x[fcname+'_quantile'],days))
+        if len(tov_df.index.names)==1:
+            to = tov_df.mean(axis =1)
+        else:
+            to = tov_df.unstack().mean(axis = 1)
         clean_factor,price = mate_al.index_mate(res_df.dropna(),Price)
         fwr = utils.compute_forward_returns(price.stack(),price)
         clean_factor[str(days)+'D'] = fwr[str(days)+'D']
         clean_factor = clean_factor.reset_index()
         clean_factor['date'] = clean_factor['date'].astype(str)
         clean_factor = clean_factor.set_index(['date','asset']).dropna()
         if index_price is not None:
@@ -660,18 +664,18 @@
         direction_dict = {}
         self.AutoMatic_DirCheck(dir_+'direction/')
         for fc in list(neu_factors):
             res_df = self.sst.factor_prepare(neu_factors,fc,self.quantiles,self.qcut)
             if self.weighted_method == 'cap_weighted':
                 res_df['cap'] = self.cap
             qreturn = self.sst.factor_ret_test_sheet(self.weighted_method,self.base_index,fc,res_df,self.Price,self.days,dir_+'/direction/',self.demean)[0]
-            if qreturn[1].sum()<= qreturn[self.quantiles].sum():
+            if qreturn[list(qreturn)[0]].sum()<= qreturn[self.quantiles].sum():
                 print(fc+'是正向因子')
                 direction_dict[fc] = 1
-            if qreturn[1].sum() > qreturn[self.quantiles].sum():
+            if qreturn[list(qreturn)[0]].sum() > qreturn[self.quantiles].sum():
                 print(fc+'是负向因子')
                 neu_factors[fc]*=-1
                 direction_dict[fc] = -1
         self.AutoMatic_DirCheck(dir_+'direction/redirection/')
         neu_factors = self.mft.mat_normlize(neu_factors)
         for fc in list(neu_factors):
             res_df = self.sst.factor_prepare(neu_factors,fc,self.quantiles,self.qcut)
```

### Comparing `Alpha_Rabbit-1.4.5/Alpha_Rabbit/Factor_Calculator.py` & `Alpha_Rabbit-1.4.6/Alpha_Rabbit/Factor_Calculator.py`

 * *Files identical despite different names*

### Comparing `Alpha_Rabbit-1.4.5/Alpha_Rabbit/Factor_Def_and_Get_Method.py` & `Alpha_Rabbit-1.4.6/Alpha_Rabbit/Factor_Def_and_Get_Method.py`

 * *Files identical despite different names*

### Comparing `Alpha_Rabbit-1.4.5/Alpha_Rabbit/trade_strategy.py` & `Alpha_Rabbit-1.4.6/Alpha_Rabbit/trade_strategy.py`

 * *Files identical despite different names*

### Comparing `Alpha_Rabbit-1.4.5/Alpha_Rabbit.egg-info/PKG-INFO` & `Alpha_Rabbit-1.4.6/Alpha_Rabbit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Alpha-Rabbit
-Version: 1.4.5
+Version: 1.4.6
 Summary: Alpha_Rabbit
 Home-page: UNKNOWN
 Author: lijiongting
 Author-email: 448986334@qq.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `Alpha_Rabbit-1.4.5/LICENSE.txt` & `Alpha_Rabbit-1.4.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Alpha_Rabbit-1.4.5/PKG-INFO` & `Alpha_Rabbit-1.4.6/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Alpha_Rabbit
-Version: 1.4.5
+Version: 1.4.6
 Summary: Alpha_Rabbit
 Home-page: UNKNOWN
 Author: lijiongting
 Author-email: 448986334@qq.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `Alpha_Rabbit-1.4.5/setup.py` & `Alpha_Rabbit-1.4.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="Alpha_Rabbit",
-    version="1.4.5",
+    version="1.4.6",
     author="lijiongting",
     author_email="448986334@qq.com",
     description="Alpha_Rabbit",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="MIT",
     url="",
```

