# Comparing `tmp/statstests-1.0.4-py3-none-any.whl.zip` & `tmp/statstests-1.0.5.dev3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,20 @@
-Zip file size: 10424 bytes, number of entries: 16
+Zip file size: 16811 bytes, number of entries: 18
 -rw-rw-r--  2.0 unx        0 b- defN 22-Sep-15 20:09 statstests/__init__.py
 -rw-rw-r--  2.0 unx     5183 b- defN 23-Feb-13 20:04 statstests/process.py
--rw-rw-r--  2.0 unx     5091 b- defN 22-Sep-20 14:30 statstests/tests.py
+-rw-rw-r--  2.0 unx    10583 b- defN 23-Jul-03 17:09 statstests/tests.py
 -rw-rw-r--  2.0 unx        0 b- defN 22-Sep-20 13:23 statstests/datasets/__init__.py
 -rw-rw-r--  2.0 unx      561 b- defN 22-Sep-20 13:16 statstests/datasets/util.py
 -rw-rw-r--  2.0 unx      117 b- defN 22-Sep-20 13:27 statstests/datasets/bebes/__init__.py
 -rwxrwxrwx  2.0 unx      750 b- defN 22-Sep-20 13:10 statstests/datasets/bebes/bebes.csv
+-rw-rw-r--  2.0 unx      124 b- defN 23-Jul-03 17:15 statstests/datasets/corruption/__init__.py
+-rwxrwxrwx  2.0 unx    12135 b- defN 23-Jul-02 15:20 statstests/datasets/corruption/corruption.csv
 -rw-rw-r--  2.0 unx      120 b- defN 22-Sep-20 13:43 statstests/datasets/empresas/__init__.py
 -rwxrwxrwx  2.0 unx     4304 b- defN 22-Sep-20 13:07 statstests/datasets/empresas/empresas.csv
--rw-rw-r--  2.0 unx       36 b- defN 23-Feb-14 13:51 statstests-1.0.4.dist-info/AUTHORS
--rw-rw-r--  2.0 unx     1049 b- defN 23-Feb-14 13:51 statstests-1.0.4.dist-info/LICENSE.txt
--rw-rw-r--  2.0 unx     1506 b- defN 23-Feb-14 13:51 statstests-1.0.4.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Feb-14 13:51 statstests-1.0.4.dist-info/WHEEL
--rw-rw-r--  2.0 unx       47 b- defN 23-Feb-14 13:51 statstests-1.0.4.dist-info/pbr.json
--rw-rw-r--  2.0 unx       11 b- defN 23-Feb-14 13:51 statstests-1.0.4.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1360 b- defN 23-Feb-14 13:51 statstests-1.0.4.dist-info/RECORD
-16 files, 20227 bytes uncompressed, 8146 bytes compressed:  59.7%
+-rw-rw-r--  2.0 unx       96 b- defN 23-Jul-10 11:22 statstests-1.0.5.dev3.dist-info/AUTHORS
+-rw-rw-r--  2.0 unx     1049 b- defN 23-Jul-10 11:22 statstests-1.0.5.dev3.dist-info/LICENSE.txt
+-rw-rw-r--  2.0 unx     1638 b- defN 23-Jul-10 11:22 statstests-1.0.5.dev3.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jul-10 11:22 statstests-1.0.5.dev3.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       47 b- defN 23-Jul-10 11:22 statstests-1.0.5.dev3.dist-info/pbr.json
+-rw-rw-r--  2.0 unx       11 b- defN 23-Jul-10 11:22 statstests-1.0.5.dev3.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1597 b- defN 23-Jul-10 11:22 statstests-1.0.5.dev3.dist-info/RECORD
+18 files, 38407 bytes uncompressed, 14137 bytes compressed:  63.2%
```

## zipnote {}

```diff
@@ -15,35 +15,41 @@
 
 Filename: statstests/datasets/bebes/__init__.py
 Comment: 
 
 Filename: statstests/datasets/bebes/bebes.csv
 Comment: 
 
+Filename: statstests/datasets/corruption/__init__.py
+Comment: 
+
+Filename: statstests/datasets/corruption/corruption.csv
+Comment: 
+
 Filename: statstests/datasets/empresas/__init__.py
 Comment: 
 
 Filename: statstests/datasets/empresas/empresas.csv
 Comment: 
 
-Filename: statstests-1.0.4.dist-info/AUTHORS
+Filename: statstests-1.0.5.dev3.dist-info/AUTHORS
 Comment: 
 
-Filename: statstests-1.0.4.dist-info/LICENSE.txt
+Filename: statstests-1.0.5.dev3.dist-info/LICENSE.txt
 Comment: 
 
-Filename: statstests-1.0.4.dist-info/METADATA
+Filename: statstests-1.0.5.dev3.dist-info/METADATA
 Comment: 
 
-Filename: statstests-1.0.4.dist-info/WHEEL
+Filename: statstests-1.0.5.dev3.dist-info/WHEEL
 Comment: 
 
-Filename: statstests-1.0.4.dist-info/pbr.json
+Filename: statstests-1.0.5.dev3.dist-info/pbr.json
 Comment: 
 
-Filename: statstests-1.0.4.dist-info/top_level.txt
+Filename: statstests-1.0.5.dev3.dist-info/top_level.txt
 Comment: 
 
-Filename: statstests-1.0.4.dist-info/RECORD
+Filename: statstests-1.0.5.dev3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## statstests/tests.py

```diff
@@ -1,15 +1,19 @@
 import numpy as np
 from scipy import stats
-import pandas as pd  # manipulação de dado em formato de dataframe
-import statsmodels.api as sm  # biblioteca de modelagem estatística
+import pandas as pd
+import statsmodels.api as sm
 import statsmodels.formula.api as smf
-   
-def shapiro_francia(array):
+from statsmodels.discrete.count_model import ZeroInflatedPoisson, ZeroInflatedNegativeBinomialP
+from statsmodels.discrete.discrete_model import Poisson, NegativeBinomial
+from scipy.stats import norm
+from typing import Union
+
 
+def shapiro_francia(array):
     r"""
 
     The statistical test of Shapiro-Francia considers the squared 
     correlation between the ordered sample values and the (approximated) 
     expected ordered quantiles from the standard normal distribution. 
 
     The p-value is computed from the formula given by Royston (1993).
@@ -57,39 +61,40 @@
             n = float(len(n))
         except TypeError:
             n = float(n)
         return (np.arange(n) + 1 - a)/(n + 1 - 2*a)
 
     x = np.sort(array)
     n = x.size
-    y = stats.norm.ppf(ppoints(n, a = 3/8))
+    y = stats.norm.ppf(ppoints(n, a=3/8))
     W, _ = np.square(stats.pearsonr(x, y))
     u = np.log(n)
     v = np.log(u)
     mu = -1.2725 + 1.0521 * (v - u)
     sig = 1.0308 - 0.26758 * (v + 2/u)
     z = (np.log(1 - W) - mu)/sig
     pval = stats.norm.sf(z)
-   
+
     dic = {}
 
     dic["method"] = "Shapiro-Francia normality test"
     dic["statistics W"] = W
     dic["statistics z"] = z
     dic["p-value"] = pval
 
     for key, value in dic.items():
         print(key, ' : ', value)
 
     return dic
 
+
 def overdisp(model, data):
     """
     Overdisp test for Statsmodels GLM Poisson model
-    
+
     """
 
     # dictionary that identifies the type of the inputed model
     models_types = {
         "<class 'statsmodels.genmod.generalized_linear_model.GLM'>": "GLM"}
 
     try:
@@ -149,8 +154,145 @@
 
     print("==================Result======================== \n")
     print(f"p-value: {modelo_auxiliar.pvalues[0]} \n")
 
     if modelo_auxiliar.pvalues[0] > 0.05:
         print("Indicates equidispersion at 95% confidence level")
     else:
-        print("Indicates overdispersion at 95% confidence level")
+        print("Indicates overdispersion at 95% confidence level")
+
+
+def vuong_test(m1: Union[Poisson, NegativeBinomial], m2: Union[ZeroInflatedPoisson, ZeroInflatedNegativeBinomialP]):
+    """    
+    Module to perform Vuong test for identification of zero inflation in count data regression models.
+
+    The new Python command vuong_test of the package statstests.tests reports the results of the Voung test.
+
+    The Vuong statistical test specifies that the Vuong (1989) test of ZIP or ZINB versus Poisson or negative binomial, 
+    respectively, be reported. This test statistic has a standard normal distribution with large values favoring 
+    ZIP or ZINB models over Poisson or negative binomial regression models, respectively.
+
+    .. ipython:: python
+
+        import pandas as pd
+        import statsmodels.api as sm
+        from statstests.datasets import corruption
+        from statstests.tests import vuong_test
+        from statsmodels.discrete.count_model import ZeroInflatedNegativeBinomialP, ZeroInflatedPoisson
+        from statsmodels.discrete.discrete_model import Poisson, NegativeBinomial
+        import warnings
+        warnings.filterwarnings('ignore')
+
+        # import corruption dataset
+        df = corruption.get_data()
+
+        #Definição da variável dependente (voltando ao dataset 'df_corruption')
+        y = df.violations
+
+        #Definição das variáveis preditoras que entrarão no componente de contagem
+        x = df[['staff','post','corruption']]
+        X = sm.add_constant(x)
+
+        X = pd.get_dummies(X, columns=['post'], drop_first=True)
+        X["post_yes"] = X["post_yes"].astype("int")
+
+        # Estimação do modelo poisson
+        modelo_poisson = Poisson(endog=y, exog=X).fit()
+
+        #Parâmetros do modelo_poisson
+        print(modelo_poisson.summary())
+
+        # Estimação do modelo poisson
+        modelo_bneg = NegativeBinomial(endog=y, exog=X, loglike_method='nb2').fit()
+
+        #Parâmetros do modelo_poisson
+        print(modelo_bneg.summary())
+
+        #Definição das variáveis preditoras que entrarão no componente de contagem
+        x1 = df[['staff','post','corruption']]
+        X1 = sm.add_constant(x1)
+
+        #Definição das variáveis preditoras que entrarão no componente logit (inflate)
+        x2 = df[['corruption']]
+        X2 = sm.add_constant(x2)
+
+        #Se estimarmos o modelo sem dummizar as variáveis categórias, o modelo retorna
+        #um erro
+        X1 = pd.get_dummies(X1, columns=['post'], drop_first=True, dtype='int')
+
+        #Estimação do modelo ZIP pela função 'ZeroInflatedPoisson' do pacote
+        #'Statsmodels'
+
+        #Estimação do modelo ZIP
+        #O argumento 'exog_infl' corresponde às variáveis que entram no componente
+        #logit (inflate)
+        # modelo_zip = ZeroInflatedPoisson(y, 
+        #                                 X1, 
+        #                                 exog_infl=X2,
+        #                                 inflation='logit').fit(maxiter=1000000000)
+
+        # #Parâmetros do modelo
+        # print(modelo_zip.summary())
+
+        # vuong_test(modelo_poisson, modelo_zip)
+
+    """
+
+    supported_models = [ZeroInflatedPoisson,
+                        ZeroInflatedNegativeBinomialP,
+                        Poisson,
+                        NegativeBinomial]
+
+    if type(m1.model) not in supported_models:
+        raise ValueError(f"Model type not supported for first parameter. List of supported models: (ZeroInflatedPoisson, ZeroInflatedNegativeBinomialP, Poisson, NegativeBinomial) from statsmodels discrete collection.")
+
+    if type(m2.model) not in supported_models:
+        raise ValueError(f"Model type not supported for second parameter. List of supported models: (ZeroInflatedPoisson, ZeroInflatedNegativeBinomialP, Poisson, NegativeBinomial) from statsmodels discrete collection.")
+
+    # Extração das variáveis dependentes dos modelos
+    m1_y = m1.model.endog
+    m2_y = m2.model.endog
+
+    m1_n = len(m1_y)
+    m2_n = len(m2_y)
+
+    if m1_n == 0 or m2_n == 0:
+        raise ValueError("Could not extract dependent variables from models.")
+
+    if m1_n != m2_n:
+        raise ValueError("Models appear to have different numbers of observations.\n"
+                         f"Model 1 has {m1_n} observations.\n"
+                         f"Model 2 has {m2_n} observations.")
+
+    if np.any(m1_y != m2_y):
+        raise ValueError(
+            "Models appear to have different values on dependent variables.")
+
+    m1_linpred = pd.DataFrame(m1.predict(which="prob"))
+    m2_linpred = pd.DataFrame(m2.predict(which="prob"))
+
+    m1_probs = np.repeat(np.nan, m1_n)
+    m2_probs = np.repeat(np.nan, m2_n)
+
+    which_col_m1 = [list(m1_linpred.columns).index(x) if x in list(
+        m1_linpred.columns) else None for x in m1_y]
+    which_col_m2 = [list(m2_linpred.columns).index(x) if x in list(
+        m2_linpred.columns) else None for x in m2_y]
+
+    for i, v in enumerate(m1_probs):
+        m1_probs[i] = m1_linpred.iloc[i, which_col_m1[i]]
+
+    for i, v in enumerate(m2_probs):
+        m2_probs[i] = m2_linpred.iloc[i, which_col_m2[i]]
+
+    lm1p = np.log(m1_probs)
+    lm2p = np.log(m2_probs)
+
+    m = lm1p - lm2p
+
+    v = np.sum(m) / (np.std(m) * np.sqrt(len(m)))
+
+    pval = 1 - norm.cdf(v) if v > 0 else norm.cdf(v)
+
+    print("Vuong Non-Nested Hypothesis Test-Statistic (Raw):")
+    print(f"Vuong z-statistic: {v}")
+    print(f"p-value: {pval}")
```

## Comparing `statstests-1.0.4.dist-info/LICENSE.txt` & `statstests-1.0.5.dev3.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `statstests-1.0.4.dist-info/METADATA` & `statstests-1.0.5.dev3.dist-info/METADATA`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: statstests
-Version: 1.0.4
+Version: 1.0.5.dev3
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: Helder Prado Santos, Luiz Paulo Fávero
 Author-email: pystatstests@gmail.com
 License: MIT
 Project-URL: Source Code, https://github.com/stats-tests/statstests
 Keywords: statstests, statsmodels, statistical tests, statistical process
@@ -15,29 +15,31 @@
 Classifier: Intended Audience :: Information Technology
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 
 # About statstests
 
 statstests is a Python package that provides a complement of process and statistical tests for statsmodels statistical models.
 
 # **Installation**
 
     pip install statstests
 
 # Documentation
 
 The documentation for the latest release is at
 
-https://www...
+https://stats-tests.github.io/statstests/
 
 # Main Features
 
 - Statistical tests:
 
   - Shapiro-Francia normality test
   - Overdispersion test
```

