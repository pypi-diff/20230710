# Comparing `tmp/pyfastedit-0.0.1.tar.gz` & `tmp/pyfastedit-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfastedit-0.0.1.tar", last modified: Mon Jul 10 14:07:24 2023, max compression
+gzip compressed data, was "pyfastedit-0.0.2.tar", last modified: Mon Jul 10 14:16:34 2023, max compression
```

## Comparing `pyfastedit-0.0.1.tar` & `pyfastedit-0.0.2.tar`

### file list

```diff
@@ -1,29 +1,31 @@
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-10 14:07:24.347153 pyfastedit-0.0.1/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     5703 2023-07-10 14:07:24.347153 pyfastedit-0.0.1/PKG-INFO
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     4784 2023-07-10 14:06:24.000000 pyfastedit-0.0.1/README.md
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-10 14:07:24.283153 pyfastedit-0.0.1/fastedit/
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-10 14:07:24.295153 pyfastedit-0.0.1/fastedit/pyfastedit.egg-info/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     5703 2023-07-10 14:07:22.000000 pyfastedit-0.0.1/fastedit/pyfastedit.egg-info/PKG-INFO
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      623 2023-07-10 14:07:23.000000 pyfastedit-0.0.1/fastedit/pyfastedit.egg-info/SOURCES.txt
--rw-r--r--   0 zhengyw  (38105) domain users (10513)        1 2023-07-10 14:07:22.000000 pyfastedit-0.0.1/fastedit/pyfastedit.egg-info/dependency_links.txt
--rw-r--r--   0 zhengyw  (38105) domain users (10513)       90 2023-07-10 14:07:22.000000 pyfastedit-0.0.1/fastedit/pyfastedit.egg-info/requires.txt
--rw-r--r--   0 zhengyw  (38105) domain users (10513)       11 2023-07-10 14:07:22.000000 pyfastedit-0.0.1/fastedit/pyfastedit.egg-info/top_level.txt
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-10 14:07:24.307153 pyfastedit-0.0.1/fastedit/rome/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)       60 2023-07-10 14:06:24.000000 pyfastedit-0.0.1/fastedit/rome/__init__.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     2696 2023-07-10 14:06:23.000000 pyfastedit-0.0.1/fastedit/rome/compute_u.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     8742 2023-07-10 14:06:23.000000 pyfastedit-0.0.1/fastedit/rome/compute_v.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     5241 2023-07-10 14:06:23.000000 pyfastedit-0.0.1/fastedit/rome/repr_tools.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      623 2023-07-10 14:06:23.000000 pyfastedit-0.0.1/fastedit/rome/rome_hparams.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     6153 2023-07-10 14:06:23.000000 pyfastedit-0.0.1/fastedit/rome/rome_main.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-10 14:07:24.343153 pyfastedit-0.0.1/fastedit/utils/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)        0 2023-07-10 14:06:24.000000 pyfastedit-0.0.1/fastedit/utils/__init__.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      272 2023-07-10 14:06:24.000000 pyfastedit-0.0.1/fastedit/utils/context.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     1992 2023-07-10 14:06:24.000000 pyfastedit-0.0.1/fastedit/utils/generate.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      338 2023-07-10 14:06:24.000000 pyfastedit-0.0.1/fastedit/utils/hparams.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      755 2023-07-10 14:06:24.000000 pyfastedit-0.0.1/fastedit/utils/mtloader.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)    15518 2023-07-10 14:06:24.000000 pyfastedit-0.0.1/fastedit/utils/nethook.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      727 2023-07-10 14:06:24.000000 pyfastedit-0.0.1/fastedit/utils/prints.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      866 2023-07-10 14:06:24.000000 pyfastedit-0.0.1/fastedit/utils/template.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)       87 2023-07-10 14:06:24.000000 pyfastedit-0.0.1/pyproject.toml
--rw-r--r--   0 zhengyw  (38105) domain users (10513)       38 2023-07-10 14:07:24.347153 pyfastedit-0.0.1/setup.cfg
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     1878 2023-07-10 14:06:25.000000 pyfastedit-0.0.1/setup.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-10 14:16:34.061663 pyfastedit-0.0.2/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     5703 2023-07-10 14:16:34.061663 pyfastedit-0.0.2/PKG-INFO
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     4784 2023-07-10 14:16:27.000000 pyfastedit-0.0.2/README.md
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-10 14:16:33.921663 pyfastedit-0.0.2/fastedit/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)       80 2023-07-10 14:16:26.000000 pyfastedit-0.0.2/fastedit/__init__.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     2567 2023-07-10 14:16:24.000000 pyfastedit-0.0.2/fastedit/editor.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-10 14:16:34.037664 pyfastedit-0.0.2/fastedit/rome/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)       60 2023-07-10 14:16:25.000000 pyfastedit-0.0.2/fastedit/rome/__init__.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     2696 2023-07-10 14:16:25.000000 pyfastedit-0.0.2/fastedit/rome/compute_u.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     8742 2023-07-10 14:16:25.000000 pyfastedit-0.0.2/fastedit/rome/compute_v.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     5241 2023-07-10 14:16:25.000000 pyfastedit-0.0.2/fastedit/rome/repr_tools.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)      623 2023-07-10 14:16:25.000000 pyfastedit-0.0.2/fastedit/rome/rome_hparams.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     6153 2023-07-10 14:16:25.000000 pyfastedit-0.0.2/fastedit/rome/rome_main.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-10 14:16:34.057664 pyfastedit-0.0.2/fastedit/utils/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)        0 2023-07-10 14:16:26.000000 pyfastedit-0.0.2/fastedit/utils/__init__.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)      272 2023-07-10 14:16:25.000000 pyfastedit-0.0.2/fastedit/utils/context.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     1992 2023-07-10 14:16:25.000000 pyfastedit-0.0.2/fastedit/utils/generate.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)      338 2023-07-10 14:16:25.000000 pyfastedit-0.0.2/fastedit/utils/hparams.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)      755 2023-07-10 14:16:25.000000 pyfastedit-0.0.2/fastedit/utils/mtloader.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)    15518 2023-07-10 14:16:25.000000 pyfastedit-0.0.2/fastedit/utils/nethook.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)      727 2023-07-10 14:16:26.000000 pyfastedit-0.0.2/fastedit/utils/prints.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)      866 2023-07-10 14:16:26.000000 pyfastedit-0.0.2/fastedit/utils/template.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-10 14:16:34.061663 pyfastedit-0.0.2/pyfastedit.egg-info/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     5703 2023-07-10 14:16:33.000000 pyfastedit-0.0.2/pyfastedit.egg-info/PKG-INFO
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)      618 2023-07-10 14:16:33.000000 pyfastedit-0.0.2/pyfastedit.egg-info/SOURCES.txt
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)        1 2023-07-10 14:16:33.000000 pyfastedit-0.0.2/pyfastedit.egg-info/dependency_links.txt
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)       90 2023-07-10 14:16:33.000000 pyfastedit-0.0.2/pyfastedit.egg-info/requires.txt
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)        9 2023-07-10 14:16:33.000000 pyfastedit-0.0.2/pyfastedit.egg-info/top_level.txt
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)       87 2023-07-10 14:16:27.000000 pyfastedit-0.0.2/pyproject.toml
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)       38 2023-07-10 14:16:34.061663 pyfastedit-0.0.2/setup.cfg
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     1830 2023-07-10 14:16:27.000000 pyfastedit-0.0.2/setup.py
```

### Comparing `pyfastedit-0.0.1/PKG-INFO` & `pyfastedit-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: pyfastedit
-Version: 0.0.1
-Summary: Editing large language models within 10 Seconds
+Version: 0.0.2
+Summary: Editing large language models within 10 seconds
 Home-page: https://github.com/hiyouga/FastEdit
 Author: hiyouga
 Author-email: hiyouga@buaa.edu.cn
 License: Apache 2.0 License
 Keywords: LLM,ChatGPT,transformer,pytorch,deep learning
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `pyfastedit-0.0.1/README.md` & `pyfastedit-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `pyfastedit-0.0.1/fastedit/pyfastedit.egg-info/PKG-INFO` & `pyfastedit-0.0.2/pyfastedit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: pyfastedit
-Version: 0.0.1
-Summary: Editing large language models within 10 Seconds
+Version: 0.0.2
+Summary: Editing large language models within 10 seconds
 Home-page: https://github.com/hiyouga/FastEdit
 Author: hiyouga
 Author-email: hiyouga@buaa.edu.cn
 License: Apache 2.0 License
 Keywords: LLM,ChatGPT,transformer,pytorch,deep learning
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `pyfastedit-0.0.1/fastedit/rome/compute_u.py` & `pyfastedit-0.0.2/fastedit/rome/compute_u.py`

 * *Files identical despite different names*

### Comparing `pyfastedit-0.0.1/fastedit/rome/compute_v.py` & `pyfastedit-0.0.2/fastedit/rome/compute_v.py`

 * *Files identical despite different names*

### Comparing `pyfastedit-0.0.1/fastedit/rome/repr_tools.py` & `pyfastedit-0.0.2/fastedit/rome/repr_tools.py`

 * *Files identical despite different names*

### Comparing `pyfastedit-0.0.1/fastedit/rome/rome_hparams.py` & `pyfastedit-0.0.2/fastedit/rome/rome_hparams.py`

 * *Files identical despite different names*

### Comparing `pyfastedit-0.0.1/fastedit/rome/rome_main.py` & `pyfastedit-0.0.2/fastedit/rome/rome_main.py`

 * *Files identical despite different names*

### Comparing `pyfastedit-0.0.1/fastedit/utils/generate.py` & `pyfastedit-0.0.2/fastedit/utils/generate.py`

 * *Files identical despite different names*

### Comparing `pyfastedit-0.0.1/fastedit/utils/mtloader.py` & `pyfastedit-0.0.2/fastedit/utils/mtloader.py`

 * *Files identical despite different names*

### Comparing `pyfastedit-0.0.1/fastedit/utils/nethook.py` & `pyfastedit-0.0.2/fastedit/utils/nethook.py`

 * *Files identical despite different names*

### Comparing `pyfastedit-0.0.1/fastedit/utils/prints.py` & `pyfastedit-0.0.2/fastedit/utils/prints.py`

 * *Files identical despite different names*

### Comparing `pyfastedit-0.0.1/fastedit/utils/template.py` & `pyfastedit-0.0.2/fastedit/utils/template.py`

 * *Files identical despite different names*

### Comparing `pyfastedit-0.0.1/setup.py` & `pyfastedit-0.0.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,22 +14,21 @@
 def main():
 
     setup(
         name="pyfastedit",
         version=get_version(),
         author="hiyouga",
         author_email="hiyouga" "@" "buaa.edu.cn",
-        description="Editing large language models within 10 Seconds",
+        description="Editing large language models within 10 seconds",
         long_description=open("README.md", "r", encoding="utf-8").read(),
         long_description_content_type="text/markdown",
         keywords=["LLM", "ChatGPT", "transformer", "pytorch", "deep learning"],
         license="Apache 2.0 License",
         url="https://github.com/hiyouga/FastEdit",
-        package_dir={"": "fastedit"},
-        packages=find_packages("fastedit"),
+        packages=find_packages(),
         python_requires=">=3.8.0",
         install_requires=[
             "torch>=1.13.1",
             "transformers>=4.29.1",
             "datasets>=2.12.0",
             "accelerate>=0.19.0",
             "sentencepiece",
```

