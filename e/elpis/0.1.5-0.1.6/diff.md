# Comparing `tmp/elpis-0.1.5.tar.gz` & `tmp/elpis-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elpis-0.1.5.tar", max compression
+gzip compressed data, was "elpis-0.1.6.tar", max compression
```

## Comparing `elpis-0.1.5.tar` & `elpis-0.1.6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     4016 2022-10-24 07:29:45.092009 elpis-0.1.5/README.md
--rw-r--r--   0        0        0       22 2022-10-21 01:31:25.222537 elpis-0.1.5/elpis/__init__.py
--rw-r--r--   0        0        0      344 2022-11-03 01:04:35.786812 elpis-0.1.5/elpis/datasets/__init__.py
--rw-r--r--   0        0        0     1929 2022-10-20 07:40:51.540623 elpis-0.1.5/elpis/datasets/clean_text.py
--rw-r--r--   0        0        0     6097 2022-10-21 06:08:02.293342 elpis-0.1.5/elpis/datasets/dataset.py
--rw-r--r--   0        0        0     6143 2022-11-03 00:49:49.957014 elpis-0.1.5/elpis/datasets/extract_annotations.py
--rw-r--r--   0        0        0     5091 2022-11-03 01:04:35.787233 elpis-0.1.5/elpis/datasets/preprocessing.py
--rw-r--r--   0        0        0     2624 2022-10-24 01:39:48.726066 elpis-0.1.5/elpis/datasets/processing.py
--rw-r--r--   0        0        0      176 2022-10-20 07:54:31.088510 elpis-0.1.5/elpis/models/__init__.py
--rw-r--r--   0        0        0     1355 2022-10-20 10:24:11.645138 elpis-0.1.5/elpis/models/annotation.py
--rw-r--r--   0        0        0      866 2022-10-20 07:56:16.504202 elpis-0.1.5/elpis/models/elan_options.py
--rw-r--r--   0        0        0      188 2022-10-21 03:44:51.004209 elpis-0.1.5/elpis/trainer/__init__.py
--rw-r--r--   0        0        0     1690 2022-11-10 05:04:55.487179 elpis-0.1.5/elpis/trainer/data_collator.py
--rw-r--r--   0        0        0     2947 2022-11-04 00:06:25.201287 elpis-0.1.5/elpis/trainer/job.py
--rw-r--r--   0        0        0     2595 2022-11-11 07:07:02.723331 elpis-0.1.5/elpis/trainer/trainer.py
--rw-r--r--   0        0        0     1530 2022-11-11 08:02:06.530220 elpis-0.1.5/elpis/trainer/utils.py
--rw-r--r--   0        0        0      201 2022-11-03 01:04:35.787493 elpis-0.1.5/elpis/transcriber/__init__.py
--rw-r--r--   0        0        0     1287 2022-11-18 02:35:11.872680 elpis-0.1.5/elpis/transcriber/results.py
--rw-r--r--   0        0        0     2561 2022-11-18 02:37:37.703724 elpis-0.1.5/elpis/transcriber/transcribe.py
--rw-r--r--   0        0        0     2184 2022-10-20 08:21:23.167179 elpis-0.1.5/elpis/utils/audio.py
--rw-r--r--   0        0        0     1025 2022-11-18 02:43:21.083340 elpis-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     5123 1970-01-01 00:00:00.000000 elpis-0.1.5/setup.py
--rw-r--r--   0        0        0     4907 1970-01-01 00:00:00.000000 elpis-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     4016 2022-10-24 07:29:45.092009 elpis-0.1.6/README.md
+-rw-r--r--   0        0        0       22 2022-10-21 01:31:25.222537 elpis-0.1.6/elpis/__init__.py
+-rw-r--r--   0        0        0      344 2022-11-03 01:04:35.786812 elpis-0.1.6/elpis/datasets/__init__.py
+-rw-r--r--   0        0        0     1929 2022-10-20 07:40:51.540623 elpis-0.1.6/elpis/datasets/clean_text.py
+-rw-r--r--   0        0        0     6097 2022-10-21 06:08:02.293342 elpis-0.1.6/elpis/datasets/dataset.py
+-rw-r--r--   0        0        0     6143 2022-11-03 00:49:49.957014 elpis-0.1.6/elpis/datasets/extract_annotations.py
+-rw-r--r--   0        0        0     5091 2022-11-03 01:04:35.787233 elpis-0.1.6/elpis/datasets/preprocessing.py
+-rw-r--r--   0        0        0     2624 2022-10-24 01:39:48.726066 elpis-0.1.6/elpis/datasets/processing.py
+-rw-r--r--   0        0        0      176 2022-10-20 07:54:31.088510 elpis-0.1.6/elpis/models/__init__.py
+-rw-r--r--   0        0        0     1355 2022-10-20 10:24:11.645138 elpis-0.1.6/elpis/models/annotation.py
+-rw-r--r--   0        0        0      866 2022-10-20 07:56:16.504202 elpis-0.1.6/elpis/models/elan_options.py
+-rw-r--r--   0        0        0      188 2022-10-21 03:44:51.004209 elpis-0.1.6/elpis/trainer/__init__.py
+-rw-r--r--   0        0        0     1690 2022-11-10 05:04:55.487179 elpis-0.1.6/elpis/trainer/data_collator.py
+-rw-r--r--   0        0        0     2947 2022-11-04 00:06:25.201287 elpis-0.1.6/elpis/trainer/job.py
+-rw-r--r--   0        0        0     2860 2022-11-30 03:47:36.945019 elpis-0.1.6/elpis/trainer/trainer.py
+-rw-r--r--   0        0        0     1337 2023-07-10 01:00:46.179161 elpis-0.1.6/elpis/trainer/utils.py
+-rw-r--r--   0        0        0      201 2022-11-03 01:04:35.787493 elpis-0.1.6/elpis/transcriber/__init__.py
+-rw-r--r--   0        0        0     1287 2022-11-18 02:35:11.872680 elpis-0.1.6/elpis/transcriber/results.py
+-rw-r--r--   0        0        0     2561 2022-11-18 02:37:37.703724 elpis-0.1.6/elpis/transcriber/transcribe.py
+-rw-r--r--   0        0        0     2184 2022-10-20 08:21:23.167179 elpis-0.1.6/elpis/utils/audio.py
+-rw-r--r--   0        0        0     1025 2023-07-10 01:02:08.442152 elpis-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     5123 1970-01-01 00:00:00.000000 elpis-0.1.6/setup.py
+-rw-r--r--   0        0        0     4907 1970-01-01 00:00:00.000000 elpis-0.1.6/PKG-INFO
```

### Comparing `elpis-0.1.5/README.md` & `elpis-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `elpis-0.1.5/elpis/datasets/clean_text.py` & `elpis-0.1.6/elpis/datasets/clean_text.py`

 * *Files identical despite different names*

### Comparing `elpis-0.1.5/elpis/datasets/dataset.py` & `elpis-0.1.6/elpis/datasets/dataset.py`

 * *Files identical despite different names*

### Comparing `elpis-0.1.5/elpis/datasets/extract_annotations.py` & `elpis-0.1.6/elpis/datasets/extract_annotations.py`

 * *Files identical despite different names*

### Comparing `elpis-0.1.5/elpis/datasets/preprocessing.py` & `elpis-0.1.6/elpis/datasets/preprocessing.py`

 * *Files identical despite different names*

### Comparing `elpis-0.1.5/elpis/datasets/processing.py` & `elpis-0.1.6/elpis/datasets/processing.py`

 * *Files identical despite different names*

### Comparing `elpis-0.1.5/elpis/models/annotation.py` & `elpis-0.1.6/elpis/models/annotation.py`

 * *Files identical despite different names*

### Comparing `elpis-0.1.5/elpis/models/elan_options.py` & `elpis-0.1.6/elpis/models/elan_options.py`

 * *Files identical despite different names*

### Comparing `elpis-0.1.5/elpis/trainer/data_collator.py` & `elpis-0.1.6/elpis/trainer/data_collator.py`

 * *Files identical despite different names*

### Comparing `elpis-0.1.5/elpis/trainer/job.py` & `elpis-0.1.6/elpis/trainer/job.py`

 * *Files identical despite different names*

### Comparing `elpis-0.1.5/elpis/trainer/trainer.py` & `elpis-0.1.6/elpis/trainer/trainer.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from contextlib import nullcontext
 from pathlib import Path
 from typing import Optional
 
 from loguru import logger
 from transformers import AutoModelForCTC, AutoProcessor, Trainer
 
 from elpis.datasets import create_dataset, prepare_dataset
@@ -26,16 +27,16 @@
         cache_dir: A directory to use for caching HFT downloads and datasets.
         log_file: An optional file to write training logs to.
 
     Returns:
         A path to the folder containing the trained model.
     """
 
-    @log_to_file(log_file)
-    def _train():
+    context = log_to_file(log_file) if log_file is not None else nullcontext()
+    with context:
         logger.info("Preparing Datasets...")
         dataset = create_dataset(dataset_dir, cache_dir)
         processor = AutoProcessor.from_pretrained(job.base_model, cache_dir=cache_dir)
         dataset = prepare_dataset(dataset, processor)
         logger.info("Finished Preparing Datasets")
 
         logger.info("Downloading pretrained model...")
@@ -68,10 +69,14 @@
 
         logger.info(f"Saving model @ {output_dir}")
         trainer.save_model()
         trainer.save_state()
         processor.save_pretrained(output_dir)
         logger.info(f"Model written to disk.")
 
-        return output_dir
+        metrics = trainer.evaluate()
+        trainer.log_metrics("eval", metrics)
+        trainer.save_metrics("eval", metrics)
+        logger.info("==== Metrics ====")
+        logger.info(metrics)
 
-    return _train()
+        return output_dir
```

### Comparing `elpis-0.1.5/elpis/transcriber/results.py` & `elpis-0.1.6/elpis/transcriber/results.py`

 * *Files identical despite different names*

### Comparing `elpis-0.1.5/elpis/transcriber/transcribe.py` & `elpis-0.1.6/elpis/transcriber/transcribe.py`

 * *Files identical despite different names*

### Comparing `elpis-0.1.5/elpis/utils/audio.py` & `elpis-0.1.6/elpis/utils/audio.py`

 * *Files identical despite different names*

### Comparing `elpis-0.1.5/pyproject.toml` & `elpis-0.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "elpis"
-version = "0.1.5"
+version = "0.1.6"
 description = """\
   A library to perform automatic speech recognition with huggingface transformers.\
   """
 readme = "README.md"
 repository = "https://github.com/CoEDL/elpis_lib"
 authors = ["Harry Keightley <harrykeightley@outlook.com>"]
 keywords = ["Elpis", "huggingface", "ASR", "Automatic Speech Recognition", "CoEDL"]
```

### Comparing `elpis-0.1.5/setup.py` & `elpis-0.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
  'pedalboard>=0.6.2,<0.7.0',
  'pympi-ling>=1.70.2,<2.0.0',
  'torch>=1.12.1,<2.0.0',
  'transformers>=4.23.1,<5.0.0']
 
 setup_kwargs = {
     'name': 'elpis',
-    'version': '0.1.5',
+    'version': '0.1.6',
     'description': 'A library to perform automatic speech recognition with huggingface transformers.',
     'long_description': '# Elpis Core Library\n\nThe Core Elpis Library, providing a quick api to [:hugs: transformers](https://huggingface.co/models?pipeline_tag=automatic-speech-recognition&sort=downloads)\nfor automatic-speech-recognition.\n\nYou can use the library to:\n\n- Perform standalone inference using a pretrained HFT model.\n- Fine tune a pretrained ASR model on your own dataset.\n- Generate text and Elan files from inference results for further analysis.\n\n## Documentation\n\nDocumentation for the library can be be found [here](https://coedl.github.io/elpis_lib/index.html).\n\n## Dependencies\n\nWhile we try to be as machine-independant as possible, there are some dependencies\nyou should be aware of when using this library:\n\n- Processing datasets (`elpis.datasets.processing`) requires `librosa`, which\n  depends on having `libsndfile` installed on your computer. If you\'re using\n  elpis within a docker container, you may have to manually install\n  `libsndfile`.\n- Transcription (`elpis.transcription.transcribe`) requires `ffmpeg` if your\n  audio you\'re attempting to transcribe needs to be resampled before it can\n  be used. The default sample rate we assume is 16khz.\n- The preprocessing flow (`elpis.datasets.preprocessing`) is free of external\n  dependencies.\n\n## Installation\n\nYou can install the elpis library with:\n`pip3 install elpis`\n\n## Usage\n\nBelow are some typical examples of use cases\n\n### Standalone Inference\n\n```python\nfrom pathlib import Path\n\nfrom elpis.transcriber.results import build_text\nfrom elpis.transcriber.transcribe import build_pipeline, transcribe\n\n# Perform inference\nasr = build_pipeline(pretrained_location="facebook/wav2vec2-base-960h")\naudio = Path("<to_some_audio_file.wav>")\nannotations = transcribe(audio, asr) # Timed, per word annotation data\n\nresult = build_text(annotations) # Combine annotations to extract all text\nprint(result)\n\n# Build output files\ntext_file = output_dir / "test.txt"\nwith open(text_file, "w") as output_file:\n    output_file.write(result)\n```\n\n### Fine-tuning a Pretrained Model on Local Dataset\n\n```python\nfrom pathlib import Path\nfrom typing import List\n\nfrom elpis.datasets import Dataset\nfrom elpis.datasets.dataset import CleaningOptions\nfrom elpis.datasets.preprocessing import process_batch\nfrom elpis.models import ElanOptions, ElanTierSelector\nfrom elpis.trainer.job import TrainingJob, TrainingOptions\nfrom elpis.trainer.trainer import train\nfrom elpis.transcriber.results import build_elan, build_text\nfrom elpis.transcriber.transcribe import build_pipeline, transcribe\n\nfiles: List[Path] = [...] # A list of paths to the files to include.\n\ndataset = Dataset(\n    name="dataset",\n    files=files,\n    cleaning_options=CleaningOptions(), # Default cleaning options\n    # Elan data extraction info- required if dataset includes .eaf files.\n    elan_options=ElanOptions(\n        selection_mechanism=ElanTierSelector.NAME, selection_value="Phrase"\n    ),\n)\n\n# Setup\ntmp_path = Path(\'...\')\n\ndataset_dir = tmp_path / "dataset"\nmodel_dir = tmp_path / "model"\noutput_dir = tmp_path / "output"\n\n# Make all directories\nfor directory in dataset_dir, model_dir, output_dir:\n    directory.mkdir(exist_ok=True, parents=True)\n\n# Preprocessing\nbatches = dataset.to_batches()\nfor batch in batches:\n    process_batch(batch, dataset_dir)\n\n# Train the model\njob = TrainingJob(\n    model_name="some_model",\n    dataset_name="some_dataset",\n    options=TrainingOptions(epochs=2, learning_rate=0.001),\n    base_model="facebook/wav2vec2-base-960h"\n)\ntrain(\n    job=job,\n    output_dir=model_dir,\n    dataset_dir=dataset_dir,\n)\n\n# Perform inference with pipeline\nasr = build_pipeline(\n    pretrained_location=str(model_dir.absolute()),\n)\naudio = Path("<to_some_audio_file.wav>")\nannotations = transcribe(audio, asr)\n\n# Build output files\ntext_file = output_dir / "test.txt"\nwith open(text_file, "w") as output_file:\n    output_file.write(build_text(annotations))\n\nelan_file = output_dir / "test.eaf"\neaf = build_elan(annotations)\neaf.to_file(str(elan_file))\n\nprint(\'voila ;)\')\n```\n',
     'author': 'Harry Keightley',
     'author_email': 'harrykeightley@outlook.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/CoEDL/elpis_lib',
```

### Comparing `elpis-0.1.5/PKG-INFO` & `elpis-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elpis
-Version: 0.1.5
+Version: 0.1.6
 Summary: A library to perform automatic speech recognition with huggingface transformers.
 Home-page: https://github.com/CoEDL/elpis_lib
 Keywords: Elpis,huggingface,ASR,Automatic Speech Recognition,CoEDL
 Author: Harry Keightley
 Author-email: harrykeightley@outlook.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
```

