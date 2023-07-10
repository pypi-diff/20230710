# Comparing `tmp/autotrain-advanced-0.5.2.tar.gz` & `tmp/autotrain-advanced-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autotrain-advanced-0.5.2.tar", last modified: Fri Mar 31 11:38:34 2023, max compression
+gzip compressed data, was "autotrain-advanced-0.5.3.tar", last modified: Mon Jul 10 11:26:44 2023, max compression
```

## Comparing `autotrain-advanced-0.5.2.tar` & `autotrain-advanced-0.5.3.tar`

### file list

```diff
@@ -1,35 +1,46 @@
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-03-31 11:38:34.110867 autotrain-advanced-0.5.2/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    11357 2023-01-05 12:46:52.000000 autotrain-advanced-0.5.2/LICENSE
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1462 2023-03-31 11:38:34.110867 autotrain-advanced-0.5.2/PKG-INFO
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      485 2023-01-05 12:49:14.000000 autotrain-advanced-0.5.2/README.md
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      353 2023-03-31 11:38:34.110867 autotrain-advanced-0.5.2/setup.cfg
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2203 2023-03-27 10:58:32.000000 autotrain-advanced-0.5.2/setup.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-03-31 11:38:34.106867 autotrain-advanced-0.5.2/src/
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-03-31 11:38:34.110867 autotrain-advanced-0.5.2/src/autotrain/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      691 2023-03-31 11:38:19.000000 autotrain-advanced-0.5.2/src/autotrain/__init__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    16336 2023-03-31 09:41:05.000000 autotrain-advanced-0.5.2/src/autotrain/app.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-03-31 11:38:34.110867 autotrain-advanced-0.5.2/src/autotrain/cli/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      310 2023-02-01 13:00:34.000000 autotrain-advanced-0.5.2/src/autotrain/cli/__init__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      829 2023-02-03 10:33:55.000000 autotrain-advanced-0.5.2/src/autotrain/cli/autotrain.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2481 2023-03-28 13:37:47.000000 autotrain-advanced-0.5.2/src/autotrain/cli/run_app.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      306 2023-03-21 05:59:11.000000 autotrain-advanced-0.5.2/src/autotrain/config.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     8408 2023-03-31 10:30:50.000000 autotrain-advanced-0.5.2/src/autotrain/dataset.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     5023 2023-01-05 12:46:52.000000 autotrain-advanced-0.5.2/src/autotrain/languages.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     6081 2023-03-31 09:11:30.000000 autotrain-advanced-0.5.2/src/autotrain/params.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-03-31 11:38:34.110867 autotrain-advanced-0.5.2/src/autotrain/preprocessor/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-02-11 08:10:09.000000 autotrain-advanced-0.5.2/src/autotrain/preprocessor/__init__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2330 2023-03-18 09:49:44.000000 autotrain-advanced-0.5.2/src/autotrain/preprocessor/dreambooth.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     4062 2023-02-16 08:46:59.000000 autotrain-advanced-0.5.2/src/autotrain/preprocessor/tabular.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     4129 2023-03-31 10:31:29.000000 autotrain-advanced-0.5.2/src/autotrain/preprocessor/text.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-02-16 08:39:08.000000 autotrain-advanced-0.5.2/src/autotrain/preprocessor/vision.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     4982 2023-03-31 09:18:09.000000 autotrain-advanced-0.5.2/src/autotrain/project.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)       64 2023-01-05 12:46:52.000000 autotrain-advanced-0.5.2/src/autotrain/splits.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2649 2023-03-31 09:18:45.000000 autotrain-advanced-0.5.2/src/autotrain/tasks.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3173 2023-03-29 12:22:27.000000 autotrain-advanced-0.5.2/src/autotrain/utils.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-03-31 11:38:34.110867 autotrain-advanced-0.5.2/src/autotrain_advanced.egg-info/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1462 2023-03-31 11:38:33.000000 autotrain-advanced-0.5.2/src/autotrain_advanced.egg-info/PKG-INFO
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      836 2023-03-31 11:38:34.000000 autotrain-advanced-0.5.2/src/autotrain_advanced.egg-info/SOURCES.txt
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        1 2023-03-31 11:38:33.000000 autotrain-advanced-0.5.2/src/autotrain_advanced.egg-info/dependency_links.txt
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)       59 2023-03-31 11:38:33.000000 autotrain-advanced-0.5.2/src/autotrain_advanced.egg-info/entry_points.txt
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      821 2023-03-31 11:38:33.000000 autotrain-advanced-0.5.2/src/autotrain_advanced.egg-info/requires.txt
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)       10 2023-03-31 11:38:33.000000 autotrain-advanced-0.5.2/src/autotrain_advanced.egg-info/top_level.txt
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-10 11:26:44.794564 autotrain-advanced-0.5.3/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    11357 2023-01-05 12:46:52.000000 autotrain-advanced-0.5.3/LICENSE
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1462 2023-07-10 11:26:44.794564 autotrain-advanced-0.5.3/PKG-INFO
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      485 2023-01-05 12:49:14.000000 autotrain-advanced-0.5.3/README.md
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      354 2023-07-10 11:26:44.794564 autotrain-advanced-0.5.3/setup.cfg
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2130 2023-06-15 09:39:07.000000 autotrain-advanced-0.5.3/setup.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-10 11:26:44.790564 autotrain-advanced-0.5.3/src/
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-10 11:26:44.790564 autotrain-advanced-0.5.3/src/autotrain/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      691 2023-07-10 11:26:39.000000 autotrain-advanced-0.5.3/src/autotrain/__init__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    38472 2023-06-21 11:15:37.000000 autotrain-advanced-0.5.3/src/autotrain/app.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-10 11:26:44.794564 autotrain-advanced-0.5.3/src/autotrain/cli/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      310 2023-02-01 13:00:34.000000 autotrain-advanced-0.5.3/src/autotrain/cli/__init__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      937 2023-07-06 09:04:02.000000 autotrain-advanced-0.5.3/src/autotrain/cli/autotrain.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1268 2023-06-21 11:15:59.000000 autotrain-advanced-0.5.3/src/autotrain/cli/run_app.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    13085 2023-07-06 09:54:47.000000 autotrain-advanced-0.5.3/src/autotrain/cli/run_llm.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      306 2023-04-29 09:05:02.000000 autotrain-advanced-0.5.3/src/autotrain/config.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    12533 2023-06-20 11:50:06.000000 autotrain-advanced-0.5.3/src/autotrain/dataset.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1483 2023-04-25 18:01:52.000000 autotrain-advanced-0.5.3/src/autotrain/help.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      197 2023-04-14 11:28:41.000000 autotrain-advanced-0.5.3/src/autotrain/languages.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    17211 2023-06-21 06:25:20.000000 autotrain-advanced-0.5.3/src/autotrain/params.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-10 11:26:44.794564 autotrain-advanced-0.5.3/src/autotrain/preprocessor/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-02-11 08:10:09.000000 autotrain-advanced-0.5.3/src/autotrain/preprocessor/__init__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1741 2023-06-20 11:50:06.000000 autotrain-advanced-0.5.3/src/autotrain/preprocessor/dreambooth.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3991 2023-04-29 09:05:23.000000 autotrain-advanced-0.5.3/src/autotrain/preprocessor/tabular.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     9231 2023-04-29 09:05:46.000000 autotrain-advanced-0.5.3/src/autotrain/preprocessor/text.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     6549 2023-05-31 09:41:05.000000 autotrain-advanced-0.5.3/src/autotrain/preprocessor/vision.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     8164 2023-06-20 11:50:06.000000 autotrain-advanced-0.5.3/src/autotrain/project.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)       64 2023-01-05 12:46:52.000000 autotrain-advanced-0.5.3/src/autotrain/splits.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2779 2023-04-25 18:01:52.000000 autotrain-advanced-0.5.3/src/autotrain/tasks.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-10 11:26:44.794564 autotrain-advanced-0.5.3/src/autotrain/trainers/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-06-15 09:39:07.000000 autotrain-advanced-0.5.3/src/autotrain/trainers/__init__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1305 2023-07-05 07:53:30.000000 autotrain-advanced-0.5.3/src/autotrain/trainers/callbacks.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     7587 2023-07-06 09:51:50.000000 autotrain-advanced-0.5.3/src/autotrain/trainers/clm.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    34306 2023-06-20 15:50:18.000000 autotrain-advanced-0.5.3/src/autotrain/trainers/dreambooth.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    10026 2023-06-20 11:50:06.000000 autotrain-advanced-0.5.3/src/autotrain/trainers/image_classification.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    14726 2023-06-22 02:39:49.000000 autotrain-advanced-0.5.3/src/autotrain/trainers/lm_trainer.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     9119 2023-06-20 09:52:02.000000 autotrain-advanced-0.5.3/src/autotrain/trainers/text_classification.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     5070 2023-07-10 11:23:13.000000 autotrain-advanced-0.5.3/src/autotrain/trainers/utils.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     8242 2023-06-21 11:52:51.000000 autotrain-advanced-0.5.3/src/autotrain/utils.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-10 11:26:44.794564 autotrain-advanced-0.5.3/src/autotrain_advanced.egg-info/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1462 2023-07-10 11:26:44.000000 autotrain-advanced-0.5.3/src/autotrain_advanced.egg-info/PKG-INFO
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1187 2023-07-10 11:26:44.000000 autotrain-advanced-0.5.3/src/autotrain_advanced.egg-info/SOURCES.txt
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        1 2023-07-10 11:26:44.000000 autotrain-advanced-0.5.3/src/autotrain_advanced.egg-info/dependency_links.txt
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)       59 2023-07-10 11:26:44.000000 autotrain-advanced-0.5.3/src/autotrain_advanced.egg-info/entry_points.txt
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3069 2023-07-10 11:26:44.000000 autotrain-advanced-0.5.3/src/autotrain_advanced.egg-info/requires.txt
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)       10 2023-07-10 11:26:44.000000 autotrain-advanced-0.5.3/src/autotrain_advanced.egg-info/top_level.txt
```

### Comparing `autotrain-advanced-0.5.2/LICENSE` & `autotrain-advanced-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.5.2/PKG-INFO` & `autotrain-advanced-0.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autotrain-advanced
-Version: 0.5.2
+Version: 0.5.3
 Home-page: https://github.com/huggingface/autotrain-advanced
 Download-URL: https://github.com/huggingface/autotrain-advanced/tags
 Author: HuggingFace Inc.
 Author-email: autotrain@huggingface.co
 License: Apache 2.0
 Keywords: automl autonlp autotrain huggingface
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `autotrain-advanced-0.5.2/setup.py` & `autotrain-advanced-0.5.3/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,25 +9,17 @@
 
 DOCLINES = __doc__.split("\n")
 
 this_directory = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(this_directory, "README.md"), encoding="utf-8") as f:
     LONG_DESCRIPTION = f.read()
 
-INSTALL_REQUIRES = [
-    "loguru==0.6.0",
-    "requests==2.28.2",
-    "tqdm==4.64.1",
-    "pandas==1.5.3",
-    "huggingface_hub==0.13.2",
-    "datasets~=2.10.0",
-    "scikit-learn==1.2.2",
-    "streamlit==1.19.0",
-    "streamlit-aggrid==0.3.3",
-]
+# get INSTALL_REQUIRES from requirements.txt
+with open(os.path.join(this_directory, "requirements.txt"), encoding="utf-8") as f:
+    INSTALL_REQUIRES = f.read().splitlines()
 
 QUALITY_REQUIRE = [
     "black",
     "isort",
     "flake8==3.7.9",
 ]
```

### Comparing `autotrain-advanced-0.5.2/src/autotrain/__init__.py` & `autotrain-advanced-0.5.3/src/autotrain/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,8 +12,8 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 # Lint as: python3
 # pylint: enable=line-too-long
 
-__version__ = "0.5.2"
+__version__ = "0.5.3"
```

### Comparing `autotrain-advanced-0.5.2/src/autotrain/cli/autotrain.py` & `autotrain-advanced-0.5.3/src/autotrain/cli/autotrain.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 import argparse
 
 from .. import __version__
 from .run_app import RunAutoTrainAppCommand
+from .run_llm import RunAutoTrainLLMCommand
 
 
 def main():
     parser = argparse.ArgumentParser(
         "AutoTrain advanced CLI",
         usage="autotrain <command> [<args>]",
         epilog="For more information about a command, run: `autotrain <command> --help`",
     )
     parser.add_argument("--version", "-v", help="Display AutoTrain version", action="store_true")
     commands_parser = parser.add_subparsers(help="commands")
 
     # Register commands
     RunAutoTrainAppCommand.register_subcommand(commands_parser)
+    RunAutoTrainLLMCommand.register_subcommand(commands_parser)
 
     args = parser.parse_args()
 
     if args.version:
         print(__version__)
         exit(0)
```

### Comparing `autotrain-advanced-0.5.2/src/autotrain/preprocessor/tabular.py` & `autotrain-advanced-0.5.3/src/autotrain/preprocessor/tabular.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from dataclasses import dataclass
 from typing import Optional
 
 import pandas as pd
 from datasets import Dataset
-from loguru import logger
 from sklearn.model_selection import train_test_split
 
 
 RESERVED_COLUMNS = ["autotrain_id", "autotrain_label"]
 
 
 @dataclass
@@ -18,15 +17,14 @@
     project_name: str
     id_column: Optional[str] = None
     valid_data: Optional[pd.DataFrame] = None
     test_size: Optional[float] = 0.2
     seed: Optional[int] = 42
 
     def __post_init__(self):
-        logger.info(self.train_data.columns)
         # check if id_column and label_column are in train_data
         if self.id_column is not None:
             if self.id_column not in self.train_data.columns:
                 raise ValueError(f"{self.id_column} not in train data")
 
         if self.label_column not in self.train_data.columns:
             raise ValueError(f"{self.label_column} not in train data")
```

### Comparing `autotrain-advanced-0.5.2/src/autotrain/tasks.py` & `autotrain-advanced-0.5.3/src/autotrain/tasks.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,37 +1,38 @@
 NLP_TASKS = {
     "text_binary_classification": 1,
     "text_multi_class_classification": 2,
-    # "text_entity_extraction": 4,
-    # "text_extractive_question_answering": 5,
-    # "text_summarization": 8,
-    # "text_single_column_regression": 10,
-    # "speech_recognition": 11,
-    # "natural_language_inference": 22,
+    "text_entity_extraction": 4,
+    "text_extractive_question_answering": 5,
+    "text_summarization": 8,
+    "text_single_column_regression": 10,
+    "speech_recognition": 11,
+    "natural_language_inference": 22,
+    "lm_training": 9,
 }
 
 VISION_TASKS = {
-    # "image_binary_classification": 17,
-    # "image_multi_class_classification": 18,
-    # "image_single_column_regression": 24,
+    "image_binary_classification": 17,
+    "image_multi_class_classification": 18,
+    "image_single_column_regression": 24,
     "dreambooth": 25,
 }
 
 TABULAR_TASKS = {
     "tabular_binary_classification": 13,
     "tabular_multi_class_classification": 14,
     "tabular_multi_label_classification": 15,
     "tabular_single_column_regression": 16,
 }
 
 
 TASKS = {
     **NLP_TASKS,
     **VISION_TASKS,
-    # **TABULAR_TASKS,
+    **TABULAR_TASKS,
 }
 
 COLUMN_MAPPING = {
     "text_binary_classification": ("text", "label"),
     "text_multi_class_classification": ("text", "label"),
     "text_entity_extraction": ("text", "tokens"),
     "text_extractive_question_answering": ("text", "context", "question", "answer"),
@@ -43,23 +44,25 @@
     "image_multi_class_classification": ("image", "label"),
     "image_single_column_regression": ("image", "label"),
     # "dreambooth": ("image", "label"),
     "tabular_binary_classification": ("id", "label"),
     "tabular_multi_class_classification": ("id", "label"),
     "tabular_multi_label_classification": ("id", "label"),
     "tabular_single_column_regression": ("id", "label"),
+    "lm_training": ("text", "prompt_start", "prompt", "context", "response"),
 }
 
 TASK_TYPE_MAPPING = {
     "text_binary_classification": "Natural Language Processing",
     "text_multi_class_classification": "Natural Language Processing",
     "text_entity_extraction": "Natural Language Processing",
     "text_extractive_question_answering": "Natural Language Processing",
     "text_summarization": "Natural Language Processing",
     "text_single_column_regression": "Natural Language Processing",
+    "lm_training": "Natural Language Processing",
     "speech_recognition": "Natural Language Processing",
     "natural_language_inference": "Natural Language Processing",
     "image_binary_classification": "Computer Vision",
     "image_multi_class_classification": "Computer Vision",
     "image_single_column_regression": "Computer Vision",
     "dreambooth": "Computer Vision",
     "tabular_binary_classification": "Tabular",
```

### Comparing `autotrain-advanced-0.5.2/src/autotrain_advanced.egg-info/PKG-INFO` & `autotrain-advanced-0.5.3/src/autotrain_advanced.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autotrain-advanced
-Version: 0.5.2
+Version: 0.5.3
 Home-page: https://github.com/huggingface/autotrain-advanced
 Download-URL: https://github.com/huggingface/autotrain-advanced/tags
 Author: HuggingFace Inc.
 Author-email: autotrain@huggingface.co
 License: Apache 2.0
 Keywords: automl autonlp autotrain huggingface
 Classifier: Development Status :: 5 - Production/Stable
```

