# Comparing `tmp/Alpha_Rabbit-1.4.4.tar.gz` & `tmp/Alpha_Rabbit-1.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Alpha_Rabbit-1.4.4.tar", last modified: Thu Jul  6 05:54:21 2023, max compression
+gzip compressed data, was "Alpha_Rabbit-1.4.5.tar", last modified: Mon Jul 10 08:17:26 2023, max compression
```

## Comparing `Alpha_Rabbit-1.4.4.tar` & `Alpha_Rabbit-1.4.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-07-06 05:54:21.449684 Alpha_Rabbit-1.4.4/
-drwxrwxrwx   0        0        0        0 2023-07-06 05:54:21.443700 Alpha_Rabbit-1.4.4/Alpha_Rabbit/
--rw-rw-rw-   0        0        0    42315 2023-07-06 05:48:25.000000 Alpha_Rabbit-1.4.4/Alpha_Rabbit/Alpha_Rabbit.py
--rw-rw-rw-   0        0        0    13937 2023-07-06 05:48:27.000000 Alpha_Rabbit-1.4.4/Alpha_Rabbit/Factor_Calculator.py
--rw-rw-rw-   0        0        0    22658 2023-06-05 07:41:31.000000 Alpha_Rabbit-1.4.4/Alpha_Rabbit/Factor_Def_and_Get_Method.py
--rw-rw-rw-   0        0        0        0 2023-02-27 02:16:19.000000 Alpha_Rabbit-1.4.4/Alpha_Rabbit/__init__.py
--rw-rw-rw-   0        0        0     1522 2023-02-27 02:16:19.000000 Alpha_Rabbit-1.4.4/Alpha_Rabbit/trade_strategy.py
-drwxrwxrwx   0        0        0        0 2023-07-06 05:54:21.448686 Alpha_Rabbit-1.4.4/Alpha_Rabbit.egg-info/
--rw-rw-rw-   0        0        0      787 2023-07-06 05:54:21.000000 Alpha_Rabbit-1.4.4/Alpha_Rabbit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      411 2023-07-06 05:54:21.000000 Alpha_Rabbit-1.4.4/Alpha_Rabbit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-06 05:54:21.000000 Alpha_Rabbit-1.4.4/Alpha_Rabbit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-07-06 05:54:21.000000 Alpha_Rabbit-1.4.4/Alpha_Rabbit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-07-06 05:54:21.000000 Alpha_Rabbit-1.4.4/Alpha_Rabbit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-02-27 02:16:19.000000 Alpha_Rabbit-1.4.4/Alpha_Rabbit.egg-info/zip-safe
--rw-rw-rw-   0        0        0     1094 2023-02-27 02:16:19.000000 Alpha_Rabbit-1.4.4/LICENSE.txt
--rw-rw-rw-   0        0        0      787 2023-07-06 05:54:21.449684 Alpha_Rabbit-1.4.4/PKG-INFO
--rw-rw-rw-   0        0        0       69 2023-02-27 02:16:19.000000 Alpha_Rabbit-1.4.4/README.md
--rw-rw-rw-   0        0        0       85 2023-07-06 05:54:21.450686 Alpha_Rabbit-1.4.4/setup.cfg
--rw-rw-rw-   0        0        0     1229 2023-07-06 05:54:01.000000 Alpha_Rabbit-1.4.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-10 08:17:26.027681 Alpha_Rabbit-1.4.5/
+drwxrwxrwx   0        0        0        0 2023-07-10 08:17:26.019159 Alpha_Rabbit-1.4.5/Alpha_Rabbit/
+-rw-rw-rw-   0        0        0    42376 2023-07-10 08:14:29.000000 Alpha_Rabbit-1.4.5/Alpha_Rabbit/Alpha_Rabbit.py
+-rw-rw-rw-   0        0        0    13979 2023-07-10 08:16:58.000000 Alpha_Rabbit-1.4.5/Alpha_Rabbit/Factor_Calculator.py
+-rw-rw-rw-   0        0        0    22658 2023-06-05 07:41:31.000000 Alpha_Rabbit-1.4.5/Alpha_Rabbit/Factor_Def_and_Get_Method.py
+-rw-rw-rw-   0        0        0        0 2023-02-27 02:16:19.000000 Alpha_Rabbit-1.4.5/Alpha_Rabbit/__init__.py
+-rw-rw-rw-   0        0        0     1522 2023-02-27 02:16:19.000000 Alpha_Rabbit-1.4.5/Alpha_Rabbit/trade_strategy.py
+drwxrwxrwx   0        0        0        0 2023-07-10 08:17:26.026324 Alpha_Rabbit-1.4.5/Alpha_Rabbit.egg-info/
+-rw-rw-rw-   0        0        0      787 2023-07-10 08:17:25.000000 Alpha_Rabbit-1.4.5/Alpha_Rabbit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      411 2023-07-10 08:17:25.000000 Alpha_Rabbit-1.4.5/Alpha_Rabbit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-10 08:17:25.000000 Alpha_Rabbit-1.4.5/Alpha_Rabbit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-07-10 08:17:25.000000 Alpha_Rabbit-1.4.5/Alpha_Rabbit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-07-10 08:17:25.000000 Alpha_Rabbit-1.4.5/Alpha_Rabbit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-02-27 02:16:19.000000 Alpha_Rabbit-1.4.5/Alpha_Rabbit.egg-info/zip-safe
+-rw-rw-rw-   0        0        0     1094 2023-02-27 02:16:19.000000 Alpha_Rabbit-1.4.5/LICENSE.txt
+-rw-rw-rw-   0        0        0      787 2023-07-10 08:17:26.027681 Alpha_Rabbit-1.4.5/PKG-INFO
+-rw-rw-rw-   0        0        0       69 2023-02-27 02:16:19.000000 Alpha_Rabbit-1.4.5/README.md
+-rw-rw-rw-   0        0        0       85 2023-07-10 08:17:26.028727 Alpha_Rabbit-1.4.5/setup.cfg
+-rw-rw-rw-   0        0        0     1229 2023-07-10 08:17:12.000000 Alpha_Rabbit-1.4.5/setup.py
```

### Comparing `Alpha_Rabbit-1.4.4/Alpha_Rabbit/Alpha_Rabbit.py` & `Alpha_Rabbit-1.4.5/Alpha_Rabbit/Alpha_Rabbit.py`

 * *Files 1% similar despite different names*

```diff
@@ -518,15 +518,15 @@
         self.momtm = pd.DataFrame(self.momtm.stack(),columns=['momentum'])
 
         # residual volatility
         print('rise residual volatility')
         self.hist_volatility = self.returndata.ewm(halflife = 42,ignore_na = True,adjust = False).std().dropna(how = 'all')
         CMRAlist = list(self.price.rolling(252))[252:]
         self.CMRA = pd.concat(list(map(lambda x: CMRA(x,12),CMRAlist)))
-        self.Hsigma = self.olsparams['residual'].rolling(252).std()
+        self.Hsigma = self.olsparams['residual'].rolling(252,min_periods = 1).std()
         self.residual_volatility = pd.DataFrame((self.hist_volatility*0.74+self.CMRA*0.16+self.Hsigma*0.1).stack()).dropna()
         self.residual_volatility.columns = ['residual_volatility']
 
         # non-linear size
         print('rise non-linear size')
         self.nlsize = (self.size**3).dropna()
         self.nlsize.columns = ['nlsize']
@@ -534,17 +534,17 @@
         # Bp
         print('rise Bp')
         self.Bp = self.filedict['Bp'].dropna()
         
         # liquidity
         print('rise Liquidity')
         self.tvrdf = self.filedict['turnover']
-        self.liq_1m = self.tvrdf.groupby(level = 1, group_keys = False).apply(lambda x: x.sort_index().rolling(22).mean())
-        self.liq_3m = self.tvrdf.groupby(level = 1, group_keys = False).apply(lambda x: x.sort_index().rolling(74).mean())
-        self.liq_12m = self.tvrdf.groupby(level = 1, group_keys = False).apply(lambda x: x.sort_index().rolling(252).mean())
+        self.liq_1m = self.tvrdf.groupby(level = 1, group_keys = False).apply(lambda x: x.sort_index().rolling(22,min_periods =1).mean())
+        self.liq_3m = self.tvrdf.groupby(level = 1, group_keys = False).apply(lambda x: x.sort_index().rolling(74,min_periods =1).mean())
+        self.liq_12m = self.tvrdf.groupby(level = 1, group_keys = False).apply(lambda x: x.sort_index().rolling(252,min_periods =1).mean())
         self.liq = (0.35*self.liq_1m + 0.35*self.liq_3m + 0.3*self.liq_12m).dropna()
 
         print('rise Earning Yield')
         self.earning_yield = pd.concat([self.filedict['Ep'],self.filedict['Sp']],axis = 1)
         self.earning_yield['earning_yield'] = self.earning_yield['ep_ratio_ttm']*0.66+self.earning_yield['sp_ratio_ttm']*0.34
         self.earning_yield = self.earning_yield[['earning_yield']].dropna()
```

### Comparing `Alpha_Rabbit-1.4.4/Alpha_Rabbit/Factor_Calculator.py` & `Alpha_Rabbit-1.4.5/Alpha_Rabbit/Factor_Calculator.py`

 * *Files 0% similar despite different names*

```diff
@@ -199,35 +199,35 @@
     if 'qua' in factors_to_cal or factors_to_cal == 'all':
         # 分位数因子qua
         uploadfactordict['qua'] = qua(sta_del_extrm,todaydate)
 
     if 'qua20m' in factors_to_cal or factors_to_cal == 'all':
         prv_factor = _method.get_prev_days_factor_by_name('qua',notst.index[-20],conn)
         q = qua(sta_del_extrm,todaydate)
-        qua20m = pd.concat([prv_factor,q]).unstack().rolling(20).mean().iloc[-1:].stack().rename(columns = {'qua':'qua20m'})
+        qua20m = pd.concat([prv_factor,q]).unstack().rolling(20,min_periods=1).mean().iloc[-1:].stack().rename(columns = {'qua':'qua20m'})
         uploadfactordict['qua20m'] = qua20m
 
     if 'skew' in factors_to_cal or factors_to_cal == 'all':
         # 偏度因子skew
         uploadfactordict['skew'] = skew(sta_50pct,todaydate)
 
     if 'skew20m' in factors_to_cal or factors_to_cal == 'all':
         prv_factor = _method.get_prev_days_factor_by_name('skew',notst.index[-20],conn)
         sk = skew(sta_50pct,todaydate)
-        skew20m = pd.concat([prv_factor,sk]).unstack().rolling(20).mean().iloc[-1:].stack().rename(columns = {'skew':'skew20m'})
+        skew20m = pd.concat([prv_factor,sk]).unstack().rolling(20,min_periods=1).mean().iloc[-1:].stack().rename(columns = {'skew':'skew20m'})
         uploadfactordict['skew20m'] = skew20m
 
     if 's_reverse' in factors_to_cal or factors_to_cal == 'all':
         # 强反转因子
         uploadfactordict['s_reverse'] = s_reverse(sing_trade_amt,minbar,todaydate)
 
     if 's_reverse_10_sum' in factors_to_cal or factors_to_cal == 'all':
         prv_factor = _method.get_prev_days_factor_by_name('s_reverse',notst.index[-10],conn)
         sr = s_reverse(sing_trade_amt,minbar,todaydate)
-        s_reverse_10_sum = pd.concat([prv_factor,sr]).unstack().rolling(10).sum().iloc[-1:].stack().rename(columns = {'s_reverse':'s_reverse_10_sum'})
+        s_reverse_10_sum = pd.concat([prv_factor,sr]).unstack().rolling(10,min_periods=1).sum().iloc[-1:].stack().rename(columns = {'s_reverse':'s_reverse_10_sum'})
         uploadfactordict['s_reverse_10_sum'] = s_reverse_10_sum
 
     if 'daily_sta_90pct' in factors_to_cal or factors_to_cal == 'all':
         # 理想反转因子
         uploadfactordict['daily_sta_90pct'] = daily_sta_90pct(sta_del_extrm)
     
     if 'ideal_reverse' in factors_to_cal or factors_to_cal == 'all':
```

### Comparing `Alpha_Rabbit-1.4.4/Alpha_Rabbit/Factor_Def_and_Get_Method.py` & `Alpha_Rabbit-1.4.5/Alpha_Rabbit/Factor_Def_and_Get_Method.py`

 * *Files identical despite different names*

### Comparing `Alpha_Rabbit-1.4.4/Alpha_Rabbit/trade_strategy.py` & `Alpha_Rabbit-1.4.5/Alpha_Rabbit/trade_strategy.py`

 * *Files identical despite different names*

### Comparing `Alpha_Rabbit-1.4.4/Alpha_Rabbit.egg-info/PKG-INFO` & `Alpha_Rabbit-1.4.5/Alpha_Rabbit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Alpha-Rabbit
-Version: 1.4.4
+Version: 1.4.5
 Summary: Alpha_Rabbit
 Home-page: UNKNOWN
 Author: lijiongting
 Author-email: 448986334@qq.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `Alpha_Rabbit-1.4.4/LICENSE.txt` & `Alpha_Rabbit-1.4.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Alpha_Rabbit-1.4.4/PKG-INFO` & `Alpha_Rabbit-1.4.5/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Alpha_Rabbit
-Version: 1.4.4
+Version: 1.4.5
 Summary: Alpha_Rabbit
 Home-page: UNKNOWN
 Author: lijiongting
 Author-email: 448986334@qq.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `Alpha_Rabbit-1.4.4/setup.py` & `Alpha_Rabbit-1.4.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="Alpha_Rabbit",
-    version="1.4.4",
+    version="1.4.5",
     author="lijiongting",
     author_email="448986334@qq.com",
     description="Alpha_Rabbit",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="MIT",
     url="",
```

