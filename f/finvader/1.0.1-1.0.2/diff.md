# Comparing `tmp/finvader-1.0.1.tar.gz` & `tmp/finvader-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "finvader-1.0.1.tar", last modified: Wed Jun 21 23:05:50 2023, max compression
+gzip compressed data, was "finvader-1.0.2.tar", last modified: Sun Jul  9 23:52:01 2023, max compression
```

## Comparing `finvader-1.0.1.tar` & `finvader-1.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-06-21 23:05:50.305246 finvader-1.0.1/
--rw-rw-rw-   0        0        0       11 2023-05-18 21:22:46.000000 finvader-1.0.1/LICENSE
--rw-rw-rw-   0        0        0     3033 2023-06-21 23:05:50.305246 finvader-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     2327 2023-05-29 19:00:12.000000 finvader-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-21 23:05:50.289502 finvader-1.0.1/finvader/
--rw-rw-rw-   0        0        0     6705 2023-05-27 17:29:37.000000 finvader-1.0.1/finvader/Henry.py
--rw-rw-rw-   0        0        0   302545 2023-05-26 21:35:39.000000 finvader-1.0.1/finvader/SentiBignomics.py
--rw-rw-rw-   0        0        0       48 2023-05-28 11:35:13.000000 finvader-1.0.1/finvader/__init__.py
--rw-rw-rw-   0        0        0     3182 2023-05-28 10:51:52.000000 finvader-1.0.1/finvader/finvader.py
-drwxrwxrwx   0        0        0        0 2023-06-21 23:05:50.305246 finvader-1.0.1/finvader.egg-info/
--rw-rw-rw-   0        0        0     3033 2023-06-21 23:05:50.000000 finvader-1.0.1/finvader.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      297 2023-06-21 23:05:50.000000 finvader-1.0.1/finvader.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-21 23:05:50.000000 finvader-1.0.1/finvader.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-06-21 23:05:50.000000 finvader-1.0.1/finvader.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-21 23:05:50.000000 finvader-1.0.1/finvader.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      551 2023-06-21 23:04:28.000000 finvader-1.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-21 23:05:50.305246 finvader-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      619 2023-06-21 23:04:28.000000 finvader-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-09 23:52:01.627190 finvader-1.0.2/
+-rw-rw-rw-   0        0        0       39 2023-07-09 23:42:01.000000 finvader-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0     3530 2023-07-09 23:52:01.627190 finvader-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2776 2023-07-09 23:50:58.000000 finvader-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-09 23:52:01.611273 finvader-1.0.2/finvader/
+-rw-rw-rw-   0        0        0     6705 2023-05-27 17:29:37.000000 finvader-1.0.2/finvader/Henry.py
+-rw-rw-rw-   0        0        0   302545 2023-05-26 21:35:39.000000 finvader-1.0.2/finvader/SentiBignomics.py
+-rw-rw-rw-   0        0        0       48 2023-07-09 23:42:01.000000 finvader-1.0.2/finvader/__init__.py
+-rw-rw-rw-   0        0        0     3182 2023-05-28 10:51:52.000000 finvader-1.0.2/finvader/finvader.py
+drwxrwxrwx   0        0        0        0 2023-07-09 23:52:01.627190 finvader-1.0.2/finvader.egg-info/
+-rw-rw-rw-   0        0        0     3530 2023-07-09 23:52:01.000000 finvader-1.0.2/finvader.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      297 2023-07-09 23:52:01.000000 finvader-1.0.2/finvader.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-09 23:52:01.000000 finvader-1.0.2/finvader.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-07-09 23:52:01.000000 finvader-1.0.2/finvader.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-09 23:52:01.000000 finvader-1.0.2/finvader.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      563 2023-07-09 23:42:01.000000 finvader-1.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-09 23:52:01.633636 finvader-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      656 2023-07-09 23:43:52.000000 finvader-1.0.2/setup.py
```

### Comparing `finvader-1.0.1/PKG-INFO` & `finvader-1.0.2/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,83 +1,74 @@
-Metadata-Version: 2.1
-Name: finvader
-Version: 1.0.1
-Summary: VADER sentiment classifier updated with financial lexicons
-Home-page: https://github.com/PetrKorab/FinVADER
-Author: Petr Koráb
-Author-email: Petr Korab <xpetrkorab@gmail.com>
-License: MIT License
-Project-URL: Homepage, https://github.com/PetrKorab/FinVADER
-Project-URL: Bug Tracker, https://github.com/PetrKorab/FinVADER/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-
-# FinVADER
-**VADER sentiment classifier updated with financial lexicons**
-
-
-**VADER** *(Valence Aware Dictionary and sEntiment Reasoner)* is a mainstream model for sentiment analysis using a 
-general-language human-curated lexicon, including linguistic features expressed on social media. As such, the model works
-worse on texts that use domain-specific language, such as finance or economics.
-
-**FinVADER** improves VADER's classification accuracy, including two finance lexicons: [SentiBignomics](https://github.com/consose/SentiBigNomics),
-and [Henry's word list](https://journals.sagepub.com/doi/10.1177/0021943608319388). *SentiBigNomics* is a detailed financial lexicon for aspect-based sentiment analysis with 
-approximately 7300 terms containing a polarity score ranging in [-1,1] for each item. *Henry's lexicon* covers 189 words 
-appearing in the company earnings press releases. 
-
-FinVADER outperforms VADER on Financial PhraseBank data: 
-
-![finvader_accuracy](https://github.com/PetrKorab/FinVADER/assets/62357254/6f464bb2-1d9c-4cb7-ba63-f535c6a1fda6)
-![vader_accuracy](https://github.com/PetrKorab/FinVADER/assets/62357254/6bc4080b-ce1a-499f-9dbd-de8cf8f1ecdc)
-
-The code for this benchmark test is [here](https://github.com/PetrKorab/FinVADER/blob/main/finvader_benchmark.ipynb)
-
-**** 
-
-
-## Installation
-
-Arabica requires [Python 3.8 - 3.11](https://www.python.org/downloads/), and [NLTK](http://www.nltk.org). 
-
-To install using pip, use:
-
-`pip install finvader`
-
-
-## Usage
-
-* **Import the library**:
-
-
-``` python
-from finvader import finvader
-```
-
-* **Select lexicons:**
-
-
-``` python
-def finvader(text = 'str',                    # Text
-             indicator = 'str',               # VADER' indicator: 'pos'/'neg'/'neu'/'compound' 
-             use_sentibignomics: bool= False, # Use SentiBignomics lexicon
-             use_henry: bool= False):         # Use Henry's lexicon
-) 
-```
-
-* **Use the classifier:**
-
-``` python
-text = "The period's sales dropped to EUR 30.6 m from EUR 38.3 m, according to the interim report, released today."
-
-scores = finvader(text, 
-                  use_sentibignomics = True, 
-                  use_henry = True, 
-                  indicator = 'compound' )
-```
-
-
-Please visit [here](https://github.com/PetrKorab/finvader/issues) for any questions, issues, bugs, and suggestions.
+# FinVADER
+**VADER sentiment classifier updated with financial lexicons**
+
+
+**VADER** *(Valence Aware Dictionary and sEntiment Reasoner)* is a mainstream model for sentiment analysis using a 
+general-language human-curated lexicon, including linguistic features expressed on social media. As such, the model works
+worse on texts that use domain-specific language, such as finance or economics.
+
+**FinVADER** improves VADER's classification accuracy, including two finance lexicons: [SentiBignomics](https://github.com/consose/SentiBigNomics),
+and [Henry's word list](https://journals.sagepub.com/doi/10.1177/0021943608319388). *SentiBigNomics* is a detailed financial lexicon for aspect-based sentiment analysis with 
+approximately 7300 terms containing a polarity score ranging in [-1,1] for each item. *Henry's lexicon* covers 189 words 
+appearing in the company earnings press releases. 
+
+FinVADER outperforms VADER on Financial PhraseBank data: 
+
+![finvader_accuracy](https://github.com/PetrKorab/FinVADER/assets/62357254/6f464bb2-1d9c-4cb7-ba63-f535c6a1fda6)
+![vader_accuracy](https://github.com/PetrKorab/FinVADER/assets/62357254/6bc4080b-ce1a-499f-9dbd-de8cf8f1ecdc)
+
+The code for this benchmark test is [here](https://github.com/PetrKorab/FinVADER/blob/main/finvader_benchmark.ipynb)
+
+**** 
+
+
+## Installation
+
+FinVADER requires [Python 3.8 - 3.11](https://www.python.org/downloads/), and [NLTK](http://www.nltk.org). 
+
+To install using pip, use:
+
+`pip install finvader`
+
+
+## Usage
+
+* **Import the library**:
+
+
+``` python
+from finvader import finvader
+```
+
+* **Select lexicons:**
+
+
+``` python
+def finvader(text = 'str',                    # Text
+             indicator = 'str',               # VADER' indicator: 'pos'/'neg'/'neu'/'compound' 
+             use_sentibignomics: bool= False, # Use SentiBignomics lexicon
+             use_henry: bool= False):         # Use Henry's lexicon
+) 
+```
+
+* **Use the classifier:**
+
+``` python
+text = "The period's sales dropped to EUR 30.6 m from EUR 38.3 m, according to the interim report, released today."
+
+scores = finvader(text, 
+                  use_sentibignomics = True, 
+                  use_henry = True, 
+                  indicator = 'compound' )
+```
+
+## Documentation, examples and tutorials
+
+For examples of coding, read these  tutorials:
+
+**FinVADER: Sentiment Analysis for Financial Applications** [here](https://medium.com/python-in-plain-english/finvader-sentiment-analysis-for-financial-applications-6ab3c08840b4)
+
+**Fine-tuning VADER Classifier with Domain-specific Lexicons** [here](https://medium.com/mlearning-ai/fine-tuning-vader-classifier-with-domain-specific-lexicons-1b23f6882f2)
+
+---
+
+Please visit [here](https://github.com/PetrKorab/finvader/issues) for any questions, issues, bugs, and suggestions.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `finvader-1.0.1/finvader/Henry.py` & `finvader-1.0.2/finvader/Henry.py`

 * *Files identical despite different names*

### Comparing `finvader-1.0.1/finvader/SentiBignomics.py` & `finvader-1.0.2/finvader/SentiBignomics.py`

 * *Files identical despite different names*

### Comparing `finvader-1.0.1/finvader/finvader.py` & `finvader-1.0.2/finvader/finvader.py`

 * *Files identical despite different names*

### Comparing `finvader-1.0.1/finvader.egg-info/PKG-INFO` & `finvader-1.0.2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: finvader
-Version: 1.0.1
+Version: 1.0.2
 Summary: VADER sentiment classifier updated with financial lexicons
 Home-page: https://github.com/PetrKorab/FinVADER
 Author: Petr Koráb
 Author-email: Petr Korab <xpetrkorab@gmail.com>
-License: MIT License
+License: OSI Approved :: Apache Software License
 Project-URL: Homepage, https://github.com/PetrKorab/FinVADER
 Project-URL: Bug Tracker, https://github.com/PetrKorab/FinVADER/issues
 Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
+Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-
 # FinVADER
 **VADER sentiment classifier updated with financial lexicons**
 
 
 **VADER** *(Valence Aware Dictionary and sEntiment Reasoner)* is a mainstream model for sentiment analysis using a 
 general-language human-curated lexicon, including linguistic features expressed on social media. As such, the model works
 worse on texts that use domain-specific language, such as finance or economics.
@@ -37,15 +36,15 @@
 The code for this benchmark test is [here](https://github.com/PetrKorab/FinVADER/blob/main/finvader_benchmark.ipynb)
 
 **** 
 
 
 ## Installation
 
-Arabica requires [Python 3.8 - 3.11](https://www.python.org/downloads/), and [NLTK](http://www.nltk.org). 
+FinVADER requires [Python 3.8 - 3.11](https://www.python.org/downloads/), and [NLTK](http://www.nltk.org). 
 
 To install using pip, use:
 
 `pip install finvader`
 
 
 ## Usage
@@ -75,9 +74,18 @@
 
 scores = finvader(text, 
                   use_sentibignomics = True, 
                   use_henry = True, 
                   indicator = 'compound' )
 ```
 
+## Documentation, examples and tutorials
+
+For examples of coding, read these  tutorials:
+
+**FinVADER: Sentiment Analysis for Financial Applications** [here](https://medium.com/python-in-plain-english/finvader-sentiment-analysis-for-financial-applications-6ab3c08840b4)
+
+**Fine-tuning VADER Classifier with Domain-specific Lexicons** [here](https://medium.com/mlearning-ai/fine-tuning-vader-classifier-with-domain-specific-lexicons-1b23f6882f2)
+
+---
 
 Please visit [here](https://github.com/PetrKorab/finvader/issues) for any questions, issues, bugs, and suggestions.
```

### Comparing `finvader-1.0.1/pyproject.toml` & `finvader-1.0.2/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 
 [project]
 name = "finvader"
-version = "1.0.1"
+version = "1.0.2"
 authors = [
   { name="Petr Korab", email="xpetrkorab@gmail.com" },
 ]
 description = "VADER sentiment classifier updated with financial lexicons"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.8"
 
 classifiers = [
     "Programming Language :: Python :: 3",
-    "License :: OSI Approved :: MIT License",
+    "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/PetrKorab/FinVADER"
 "Bug Tracker" = "https://github.com/PetrKorab/FinVADER/issues"
```

### Comparing `finvader-1.0.1/setup.py` & `finvader-1.0.2/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     description = fh.read()
 
     setuptools.setup(
         name="finvader",
-        version="1.0.1",
+        version="1.0.2",
         author="Petr Koráb",
         author_email="xpetrkorab@gmail.com",
         packages=["finvader"],
-        description="Python package for exploratory text data analysis",
+        description="VADER sentiment classifier updated with financial lexicons",
         long_description=description,
         long_description_content_type="text/markdown",
         url="https://github.com/PetrKorab/FinVADER",
         python_requires='>=3.8',
         install_requires = ['nltk == 3.6.2'],
-        license='MIT License'
+        license='OSI Approved :: Apache Software License'
     )
```

