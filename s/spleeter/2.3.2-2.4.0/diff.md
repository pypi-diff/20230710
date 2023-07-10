# Comparing `tmp/spleeter-2.3.2.tar.gz` & `tmp/spleeter-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spleeter-2.3.2.tar", max compression
+gzip compressed data, was "spleeter-2.4.0.tar", max compression
```

## Comparing `spleeter-2.3.2.tar` & `spleeter-2.4.0.tar`

### file list

```diff
@@ -1,35 +1,34 @@
--rw-r--r--   0        0        0     1075 2022-09-07 11:39:18.394468 spleeter-2.3.2/LICENSE
--rw-r--r--   0        0        0     8423 2022-09-07 11:39:18.394468 spleeter-2.3.2/README.md
--rw-r--r--   0        0        0     2906 2022-09-07 11:39:18.406468 spleeter-2.3.2/pyproject.toml
--rw-r--r--   0        0        0      699 2022-09-07 11:39:18.406468 spleeter-2.3.2/spleeter/__init__.py
--rw-r--r--   0        0        0     8438 2022-09-07 11:39:18.406468 spleeter-2.3.2/spleeter/__main__.py
--rw-r--r--   0        0        0     1399 2022-09-07 11:39:18.406468 spleeter-2.3.2/spleeter/audio/__init__.py
--rw-r--r--   0        0        0     6509 2022-09-07 11:39:18.406468 spleeter-2.3.2/spleeter/audio/adapter.py
--rw-r--r--   0        0        0     3730 2022-09-07 11:39:18.406468 spleeter-2.3.2/spleeter/audio/convertor.py
--rw-r--r--   0        0        0     6280 2022-09-07 11:39:18.406468 spleeter-2.3.2/spleeter/audio/ffmpeg.py
--rw-r--r--   0        0        0     5896 2022-09-07 11:39:18.406468 spleeter-2.3.2/spleeter/audio/spectrogram.py
--rw-r--r--   0        0        0    21009 2022-09-07 11:39:18.406468 spleeter-2.3.2/spleeter/dataset.py
--rw-r--r--   0        0        0    20422 2022-09-07 11:39:18.406468 spleeter-2.3.2/spleeter/model/__init__.py
--rw-r--r--   0        0        0     1193 2022-09-07 11:39:18.406468 spleeter-2.3.2/spleeter/model/functions/__init__.py
--rw-r--r--   0        0        0     3028 2022-09-07 11:39:18.406468 spleeter-2.3.2/spleeter/model/functions/blstm.py
--rw-r--r--   0        0        0     7198 2022-09-07 11:39:18.406468 spleeter-2.3.2/spleeter/model/functions/unet.py
--rw-r--r--   0        0        0     2698 2022-09-07 11:39:18.406468 spleeter-2.3.2/spleeter/model/provider/__init__.py
--rw-r--r--   0        0        0     4812 2022-09-07 11:39:18.406468 spleeter-2.3.2/spleeter/model/provider/github.py
--rw-r--r--   0        0        0     3714 2022-09-07 11:39:18.406468 spleeter-2.3.2/spleeter/options.py
--rw-r--r--   0        0        0        0 2022-09-07 11:39:18.406468 spleeter-2.3.2/spleeter/py.typed
--rw-r--r--   0        0        0      718 2022-09-07 11:39:18.410468 spleeter-2.3.2/spleeter/resources/2stems-16kHz.json
--rw-r--r--   0        0        0      718 2022-09-07 11:39:18.410468 spleeter-2.3.2/spleeter/resources/2stems.json
--rw-r--r--   0        0        0      800 2022-09-07 11:39:18.410468 spleeter-2.3.2/spleeter/resources/4stems-16kHz.json
--rw-r--r--   0        0        0      800 2022-09-07 11:39:18.410468 spleeter-2.3.2/spleeter/resources/4stems.json
--rw-r--r--   0        0        0      818 2022-09-07 11:39:18.410468 spleeter-2.3.2/spleeter/resources/5stems-16kHz.json
--rw-r--r--   0        0        0      818 2022-09-07 11:39:18.410468 spleeter-2.3.2/spleeter/resources/5stems.json
--rw-r--r--   0        0        0      202 2022-09-07 11:39:18.410468 spleeter-2.3.2/spleeter/resources/__init__.py
--rw-r--r--   0        0        0      850 2022-09-07 11:39:18.410468 spleeter-2.3.2/spleeter/resources/musdb.json
--rw-r--r--   0        0        0    16003 2022-09-07 11:39:18.410468 spleeter-2.3.2/spleeter/separator.py
--rw-r--r--   0        0        0      291 2022-09-07 11:39:18.410468 spleeter-2.3.2/spleeter/types.py
--rw-r--r--   0        0        0      192 2022-09-07 11:39:18.410468 spleeter-2.3.2/spleeter/utils/__init__.py
--rw-r--r--   0        0        0     1757 2022-09-07 11:39:18.410468 spleeter-2.3.2/spleeter/utils/configuration.py
--rw-r--r--   0        0        0     1407 2022-09-07 11:39:18.410468 spleeter-2.3.2/spleeter/utils/logging.py
--rw-r--r--   0        0        0     6793 2022-09-07 11:39:18.410468 spleeter-2.3.2/spleeter/utils/tensor.py
--rw-r--r--   0        0        0     9998 1970-01-01 00:00:00.000000 spleeter-2.3.2/setup.py
--rw-r--r--   0        0        0    11295 1970-01-01 00:00:00.000000 spleeter-2.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1075 2023-07-10 10:06:32.028893 spleeter-2.4.0/LICENSE
+-rw-r--r--   0        0        0     8423 2023-07-10 10:06:32.028893 spleeter-2.4.0/README.md
+-rw-r--r--   0        0        0     2745 2023-07-10 10:06:32.040893 spleeter-2.4.0/pyproject.toml
+-rw-r--r--   0        0        0      671 2023-07-10 10:06:32.040893 spleeter-2.4.0/spleeter/__init__.py
+-rw-r--r--   0        0        0     8600 2023-07-10 10:06:32.040893 spleeter-2.4.0/spleeter/__main__.py
+-rw-r--r--   0        0        0      619 2023-07-10 10:06:32.040893 spleeter-2.4.0/spleeter/audio/__init__.py
+-rw-r--r--   0        0        0     6578 2023-07-10 10:06:32.040893 spleeter-2.4.0/spleeter/audio/adapter.py
+-rw-r--r--   0        0        0     3652 2023-07-10 10:06:32.040893 spleeter-2.4.0/spleeter/audio/convertor.py
+-rw-r--r--   0        0        0     6303 2023-07-10 10:06:32.040893 spleeter-2.4.0/spleeter/audio/ffmpeg.py
+-rw-r--r--   0        0        0     5907 2023-07-10 10:06:32.040893 spleeter-2.4.0/spleeter/audio/spectrogram.py
+-rw-r--r--   0        0        0    20953 2023-07-10 10:06:32.040893 spleeter-2.4.0/spleeter/dataset.py
+-rw-r--r--   0        0        0    19898 2023-07-10 10:06:32.040893 spleeter-2.4.0/spleeter/model/__init__.py
+-rw-r--r--   0        0        0     1247 2023-07-10 10:06:32.040893 spleeter-2.4.0/spleeter/model/functions/__init__.py
+-rw-r--r--   0        0        0     3024 2023-07-10 10:06:32.040893 spleeter-2.4.0/spleeter/model/functions/blstm.py
+-rw-r--r--   0        0        0     7446 2023-07-10 10:06:32.040893 spleeter-2.4.0/spleeter/model/functions/unet.py
+-rw-r--r--   0        0        0     2746 2023-07-10 10:06:32.040893 spleeter-2.4.0/spleeter/model/provider/__init__.py
+-rw-r--r--   0        0        0     4828 2023-07-10 10:06:32.040893 spleeter-2.4.0/spleeter/model/provider/github.py
+-rw-r--r--   0        0        0     3138 2023-07-10 10:06:32.040893 spleeter-2.4.0/spleeter/options.py
+-rw-r--r--   0        0        0        0 2023-07-10 10:06:32.040893 spleeter-2.4.0/spleeter/py.typed
+-rw-r--r--   0        0        0      718 2023-07-10 10:06:32.040893 spleeter-2.4.0/spleeter/resources/2stems-16kHz.json
+-rw-r--r--   0        0        0      718 2023-07-10 10:06:32.040893 spleeter-2.4.0/spleeter/resources/2stems.json
+-rw-r--r--   0        0        0      800 2023-07-10 10:06:32.040893 spleeter-2.4.0/spleeter/resources/4stems-16kHz.json
+-rw-r--r--   0        0        0      800 2023-07-10 10:06:32.040893 spleeter-2.4.0/spleeter/resources/4stems.json
+-rw-r--r--   0        0        0      818 2023-07-10 10:06:32.040893 spleeter-2.4.0/spleeter/resources/5stems-16kHz.json
+-rw-r--r--   0        0        0      818 2023-07-10 10:06:32.040893 spleeter-2.4.0/spleeter/resources/5stems.json
+-rw-r--r--   0        0        0      202 2023-07-10 10:06:32.040893 spleeter-2.4.0/spleeter/resources/__init__.py
+-rw-r--r--   0        0        0      850 2023-07-10 10:06:32.040893 spleeter-2.4.0/spleeter/resources/musdb.json
+-rw-r--r--   0        0        0    12696 2023-07-10 10:06:32.040893 spleeter-2.4.0/spleeter/separator.py
+-rw-r--r--   0        0        0      279 2023-07-10 10:06:32.040893 spleeter-2.4.0/spleeter/types.py
+-rw-r--r--   0        0        0      192 2023-07-10 10:06:32.040893 spleeter-2.4.0/spleeter/utils/__init__.py
+-rw-r--r--   0        0        0     1591 2023-07-10 10:06:32.040893 spleeter-2.4.0/spleeter/utils/configuration.py
+-rw-r--r--   0        0        0     1437 2023-07-10 10:06:32.040893 spleeter-2.4.0/spleeter/utils/logging.py
+-rw-r--r--   0        0        0     6332 2023-07-10 10:06:32.040893 spleeter-2.4.0/spleeter/utils/tensor.py
+-rw-r--r--   0        0        0    10816 1970-01-01 00:00:00.000000 spleeter-2.4.0/PKG-INFO
```

### Comparing `spleeter-2.3.2/LICENSE` & `spleeter-2.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `spleeter-2.3.2/README.md` & `spleeter-2.4.0/README.md`

 * *Files identical despite different names*

### Comparing `spleeter-2.3.2/pyproject.toml` & `spleeter-2.4.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "spleeter"
-version = "2.3.2"
+version = "2.4.0"
 description = "The Deezer source separation library with pretrained models based on tensorflow."
 authors = ["Deezer Research <spleeter@deezer.com>"]
 license = "MIT License"
 readme = "README.md"
 repository = "https://github.com/deezer/spleeter"
 homepage = "https://github.com/deezer/spleeter"
 classifiers = [
@@ -42,37 +42,32 @@
     "Topic :: Utilities"
 ]
 packages = [ { include = "spleeter" } ]
 include = ["LICENSE", "spleeter/resources/*.json"]
 
 [tool.poetry.dependencies]
 python = ">=3.7.1,<3.11"
-ffmpeg-python = "0.2.0"
-norbert = "0.2.1"
+ffmpeg-python = "^0.2.0"
 httpx = {extras = ["http2"], version = "^0.19.0"}
 typer = "^0.3.2"
-librosa = "^0.8.0"
-musdb = {version = "0.3.1", optional = true}
-museval = {version = "0.3.0", optional = true}
-tensorflow = "^2.5.0"
-pandas = "^1.2"
-numpy = "^1.19.2"
-importlib-resources = {version = "^4.1.1", python = "<3.7"}
-importlib-metadata = {version = "^3.0.0", python = "<3.8"}
-llvmlite = "^0.38.0"
-protobuf = "^3.19.4"
+musdb = {version = "^0.4.0", optional = true}
+museval = {version = "^0.4.0", optional = true}
+tensorflow = "^2.5.0, <2.10.0"
+pandas = "^1.3.0"
+norbert = "^0.2.1"
 
 [tool.poetry.dev-dependencies]
 pytest = "^6.2.1"
 isort = "^5.7.0"
-black = "^21.7"
+black = "^21.7b0"
 mypy = "^0.790"
+flake8 = "^5.0.0"
 pytest-forked = "^1.3.0"
-musdb = "0.3.1"
-museval = "0.3.0"
+musdb = "^0.4.0"
+museval = "^0.4.0"
 
 [tool.poetry.scripts]
 spleeter = 'spleeter.__main__:entrypoint'
 
 [tool.poetry.extras]
 evaluation = ["musdb", "museval"]
```

### Comparing `spleeter-2.3.2/spleeter/__init__.py` & `spleeter-2.4.0/spleeter/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 #!/usr/bin/env python
 # coding: utf8
 
 """
-    Spleeter is the Deezer source separation library with pretrained models.
-    The library is based on Tensorflow:
+Spleeter is the Deezer source separation library with pretrained models.
+The library is based on Tensorflow:
 
-    -   It provides already trained model for performing separation.
-    -   It makes it easy to train source separation model with tensorflow
-        (provided you have a dataset of isolated sources).
+-   It provides already trained model for performing separation.
+-   It makes it easy to train source separation model with tensorflow
+    (provided you have a dataset of isolated sources).
 
-    This module allows to interact easily from command line with Spleeter
-    by providing train, evaluation and source separation action.
+This module allows to interact easily from command line with Spleeter
+by providing train, evaluation and source separation action.
 """
 
 __email__ = "spleeter@deezer.com"
 __author__ = "Deezer Research"
 __license__ = "MIT License"
```

### Comparing `spleeter-2.3.2/spleeter/__main__.py` & `spleeter-2.4.0/spleeter/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,50 @@
 #!/usr/bin/env python
 # coding: utf8
 
 """
-    Python oneliner script usage.
+Python oneliner script usage.
 
-    USAGE: python -m spleeter {train,evaluate,separate} ...
+USAGE: python -m spleeter {train,evaluate,separate} ...
 
-    Notes:
-        All critical import involving TF, numpy or Pandas are deported to
-        command function scope to avoid heavy import on CLI evaluation,
-        leading to large bootstraping time.
+Notes:
+    All critical import involving TF, numpy or Pandas are deported to
+    command function scope to avoid heavy import on CLI evaluation,
+    leading to large bootstraping time.
 """
 import json
 from functools import partial
 from glob import glob
 from itertools import product
 from os.path import join
-from pathlib import Path
-from typing import Container, Dict, List, Optional
+from typing import Dict, List, Optional, Tuple
 
 # pyright: reportMissingImports=false
 # pylint: disable=import-error
 from typer import Exit, Typer
 
 from . import SpleeterError
-from .options import *
+from .audio import Codec
+from .options import (
+    AudioAdapterOption,
+    AudioBitrateOption,
+    AudioCodecOption,
+    AudioDurationOption,
+    AudioInputArgument,
+    AudioInputOption,
+    AudioOffsetOption,
+    AudioOutputOption,
+    FilenameFormatOption,
+    ModelParametersOption,
+    MUSDBDirectoryOption,
+    MWFOption,
+    TrainingDataDirectoryOption,
+    VerboseOption,
+    VersionOption,
+)
 from .utils.logging import configure_logger, logger
 
 # pylint: enable=import-error
 
 spleeter: Typer = Typer(add_completion=False, no_args_is_help=True, short_help="-h")
 """ CLI application. """
 
@@ -39,32 +55,31 @@
 ) -> None:
     pass
 
 
 @spleeter.command(no_args_is_help=True)
 def train(
     adapter: str = AudioAdapterOption,
-    data: Path = TrainingDataDirectoryOption,
+    data: str = TrainingDataDirectoryOption,
     params_filename: str = ModelParametersOption,
     verbose: bool = VerboseOption,
 ) -> None:
     """
     Train a source separation model
     """
-    import tensorflow as tf
+    import tensorflow as tf  # type: ignore
 
     from .audio.adapter import AudioAdapter
     from .dataset import get_training_dataset, get_validation_dataset
     from .model import model_fn
     from .model.provider import ModelProvider
     from .utils.configuration import load_configuration
 
     configure_logger(verbose)
     audio_adapter = AudioAdapter.get(adapter)
-    audio_path = str(data)
     params = load_configuration(params_filename)
     session_config = tf.compat.v1.ConfigProto()
     session_config.gpu_options.per_process_gpu_memory_fraction = 0.45
     estimator = tf.estimator.Estimator(
         model_fn=model_fn,
         model_dir=params["model_dir"],
         params=params,
@@ -73,39 +88,38 @@
             tf_random_seed=params["random_seed"],
             save_summary_steps=params["save_summary_steps"],
             session_config=session_config,
             log_step_count_steps=10,
             keep_checkpoint_max=2,
         ),
     )
-    input_fn = partial(get_training_dataset, params, audio_adapter, audio_path)
+    input_fn = partial(get_training_dataset, params, audio_adapter, data)
     train_spec = tf.estimator.TrainSpec(
         input_fn=input_fn, max_steps=params["train_max_steps"]
     )
-    input_fn = partial(get_validation_dataset, params, audio_adapter, audio_path)
+    input_fn = partial(get_validation_dataset, params, audio_adapter, data)
     evaluation_spec = tf.estimator.EvalSpec(
         input_fn=input_fn, steps=None, throttle_secs=params["throttle_secs"]
     )
     logger.info("Start model training")
     tf.estimator.train_and_evaluate(estimator, train_spec, evaluation_spec)
     ModelProvider.writeProbe(params["model_dir"])
     logger.info("Model training done")
 
 
 @spleeter.command(no_args_is_help=True)
 def separate(
     deprecated_files: Optional[str] = AudioInputOption,
-    files: List[Path] = AudioInputArgument,
+    files: List[str] = AudioInputArgument,
     adapter: str = AudioAdapterOption,
     bitrate: str = AudioBitrateOption,
     codec: Codec = AudioCodecOption,
     duration: float = AudioDurationOption,
     offset: float = AudioOffsetOption,
-    output_path: Path = AudioOutputOption,
-    stft_backend: STFTBackend = AudioSTFTBackendOption,
+    output_path: str = AudioOutputOption,
     filename_format: str = FilenameFormatOption,
     params_filename: str = ModelParametersOption,
     mwf: bool = MWFOption,
     verbose: bool = VerboseOption,
 ) -> None:
     """
     Separate audio file(s)
@@ -117,62 +131,61 @@
     if deprecated_files is not None:
         logger.error(
             "⚠️ -i option is not supported anymore, audio files must be supplied "
             "using input argument instead (see spleeter separate --help)"
         )
         raise Exit(20)
     audio_adapter: AudioAdapter = AudioAdapter.get(adapter)
-    separator: Separator = Separator(
-        params_filename, MWF=mwf, stft_backend=stft_backend
-    )
+    separator: Separator = Separator(params_filename, MWF=mwf)
+
     for filename in files:
         separator.separate_to_file(
-            str(filename),
-            str(output_path),
+            filename,
+            output_path,
             audio_adapter=audio_adapter,
             offset=offset,
             duration=duration,
             codec=codec,
             bitrate=bitrate,
             filename_format=filename_format,
             synchronous=False,
         )
     separator.join()
 
 
 EVALUATION_SPLIT: str = "test"
 EVALUATION_METRICS_DIRECTORY: str = "metrics"
-EVALUATION_INSTRUMENTS: Container[str] = ("vocals", "drums", "bass", "other")
-EVALUATION_METRICS: Container[str] = ("SDR", "SAR", "SIR", "ISR")
+EVALUATION_INSTRUMENTS: Tuple[str, ...] = ("vocals", "drums", "bass", "other")
+EVALUATION_METRICS: Tuple[str, ...] = ("SDR", "SAR", "SIR", "ISR")
 EVALUATION_MIXTURE: str = "mixture.wav"
 EVALUATION_AUDIO_DIRECTORY: str = "audio"
 
 
-def _compile_metrics(metrics_output_directory) -> Dict:
+def _compile_metrics(metrics_output_directory: str) -> Dict:
     """
     Compiles metrics from given directory and returns results as dict.
 
     Parameters:
         metrics_output_directory (str):
             Directory to get metrics from.
 
     Returns:
         Dict:
             Compiled metrics as dict.
     """
     import numpy as np
-    import pandas as pd
+    import pandas as pd  # type: ignore
 
     songs = glob(join(metrics_output_directory, "test/*.json"))
     index = pd.MultiIndex.from_tuples(
         product(EVALUATION_INSTRUMENTS, EVALUATION_METRICS),
         names=["instrument", "metric"],
     )
     pd.DataFrame([], index=["config1", "config2"], columns=index)
-    metrics = {
+    metrics: Dict = {
         instrument: {k: [] for k in EVALUATION_METRICS}
         for instrument in EVALUATION_INSTRUMENTS
     }
     for song in songs:
         with open(song, "r") as stream:
             data = json.load(stream)
         for target in data["targets"]:
@@ -188,30 +201,29 @@
                 metrics[instrument][metric].append(sdr_med)
     return metrics
 
 
 @spleeter.command(no_args_is_help=True)
 def evaluate(
     adapter: str = AudioAdapterOption,
-    output_path: Path = AudioOutputOption,
-    stft_backend: STFTBackend = AudioSTFTBackendOption,
+    output_path: str = AudioOutputOption,
     params_filename: str = ModelParametersOption,
-    mus_dir: Path = MUSDBDirectoryOption,
+    mus_dir: str = MUSDBDirectoryOption,
     mwf: bool = MWFOption,
     verbose: bool = VerboseOption,
 ) -> Dict:
     """
     Evaluate a model on the musDB test dataset
     """
     import numpy as np
 
     configure_logger(verbose)
     try:
-        import musdb
-        import museval
+        import musdb  # type: ignore
+        import museval  # type: ignore
     except ImportError:
         logger.error("Extra dependencies musdb and museval not found")
         logger.error("Please install musdb and museval first, abort")
         raise Exit(10)
     # Separate musdb sources.
     songs = glob(join(mus_dir, EVALUATION_SPLIT, "*/"))
     mixtures = [join(song, EVALUATION_MIXTURE) for song in songs]
@@ -221,15 +233,14 @@
         files=mixtures,
         adapter=adapter,
         bitrate="128k",
         codec=Codec.WAV,
         duration=600.0,
         offset=0,
         output_path=join(audio_output_directory, EVALUATION_SPLIT),
-        stft_backend=stft_backend,
         filename_format="{foldername}/{instrument}.{codec}",
         params_filename=params_filename,
         mwf=mwf,
         verbose=verbose,
     )
     # Compute metrics with musdb.
     metrics_output_directory = join(output_path, EVALUATION_METRICS_DIRECTORY)
```

### Comparing `spleeter-2.3.2/spleeter/audio/adapter.py` & `spleeter-2.4.0/spleeter/audio/adapter.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from importlib import import_module
 from pathlib import Path
 from typing import Any, Dict, List, Optional, Union
 
 # pyright: reportMissingImports=false
 # pylint: disable=import-error
 import numpy as np
-import tensorflow as tf
+import tensorflow as tf  # type: ignore
 
 from spleeter.audio import Codec
 
 from .. import SpleeterError
 from ..types import AudioDescriptor, Signal
 from ..utils.logging import logger
 
@@ -26,73 +26,73 @@
 __author__ = "Deezer Research"
 __license__ = "MIT License"
 
 
 class AudioAdapter(ABC):
     """An abstract class for manipulating audio signal."""
 
-    _DEFAULT: "AudioAdapter" = None
-    """ Default audio adapter singleton instance. """
+    _DEFAULT: Optional["AudioAdapter"] = None
+    """Default audio adapter singleton instance."""
 
     @abstractmethod
     def load(
         self,
         audio_descriptor: AudioDescriptor,
         offset: Optional[float] = None,
         duration: Optional[float] = None,
         sample_rate: Optional[float] = None,
-        dtype: np.dtype = np.float32,
+        dtype: bytes = b"float32",
     ) -> Signal:
         """
         Loads the audio file denoted by the given audio descriptor and
         returns it data as a waveform. Aims to be implemented by client.
 
         Parameters:
             audio_descriptor (AudioDescriptor):
                 Describe song to load, in case of file based audio adapter,
                 such descriptor would be a file path.
             offset (Optional[float]):
-                Start offset to load from in seconds.
+                (Optional) Start offset to load from in seconds.
             duration (Optional[float]):
-                Duration to load in seconds.
+                (Optional) Duration to load in seconds.
             sample_rate (Optional[float]):
-                Sample rate to load audio with.
-            dtype (numpy.dtype):
-                (Optional) Numpy data type to use, default to `float32`.
+                (Optional) Sample rate to load audio with.
+            dtype (bytes):
+                (Optional) Data type to use, default to `b'float32'`.
 
         Returns:
             Signal:
                 Loaded data as (wf, sample_rate) tuple.
         """
         pass
 
-    def load_tf_waveform(
+    def load_waveform(
         self,
         audio_descriptor,
         offset: float = 0.0,
         duration: float = 1800.0,
         sample_rate: int = 44100,
         dtype: bytes = b"float32",
         waveform_name: str = "waveform",
     ) -> Dict[str, Any]:
         """
         Load the audio and convert it to a tensorflow waveform.
 
         Parameters:
-            audio_descriptor ():
+            audio_descriptor (Any):
                 Describe song to load, in case of file based audio adapter,
                 such descriptor would be a file path.
             offset (float):
-                Start offset to load from in seconds.
+                (Optional) Start offset to load from in seconds.
             duration (float):
-                Duration to load in seconds.
+                (Optional) Duration to load in seconds.
             sample_rate (float):
-                Sample rate to load audio with.
+                (Optional) Sample rate to load audio with.
             dtype (bytes):
-                (Optional)data type to use, default to `b'float32'`.
+                (Optional) Data type to use, default to `b'float32'`.
             waveform_name (str):
                 (Optional) Name of the key in output dict, default to
                 `'waveform'`.
 
         Returns:
             Dict[str, Any]:
                 TF output dict with waveform as `(T x chan numpy array)`
@@ -142,59 +142,59 @@
     ) -> None:
         """
         Save the given audio data to the file denoted by the given path.
 
         Parameters:
             path (Union[Path, str]):
                 Path like of the audio file to save data in.
-            data (numpy.ndarray):
+            data (np.ndarray):
                 Waveform data to write.
             sample_rate (float):
                 Sample rate to write file in.
-            codec ():
+            codec (Codec):
                 (Optional) Writing codec to use, default to `None`.
             bitrate (str):
                 (Optional) Bitrate of the written audio file, default to
                 `None`.
         """
         pass
 
     @classmethod
-    def default(cls: type) -> "AudioAdapter":
+    def default(cls) -> "AudioAdapter":
         """
         Builds and returns a default audio adapter instance.
 
         Returns:
             AudioAdapter:
                 Default adapter instance to use.
         """
         if cls._DEFAULT is None:
             from .ffmpeg import FFMPEGProcessAudioAdapter
 
             cls._DEFAULT = FFMPEGProcessAudioAdapter()
         return cls._DEFAULT
 
     @classmethod
-    def get(cls: type, descriptor: str) -> "AudioAdapter":
+    def get(cls, descriptor: str) -> "AudioAdapter":
         """
         Load dynamically an AudioAdapter from given class descriptor.
 
         Parameters:
             descriptor (str):
                 Adapter class descriptor (module.Class)
 
         Returns:
             AudioAdapter:
                 Created adapter instance.
         """
         if not descriptor:
             return cls.default()
-        module_path: List[str] = descriptor.split(".")
-        adapter_class_name: str = module_path[-1]
-        module_path: str = ".".join(module_path[:-1])
+        module_desc: List[str] = descriptor.split(".")
+        adapter_class_name: str = module_desc[-1]
+        module_path: str = ".".join(module_desc[:-1])
         adapter_module = import_module(module_path)
         adapter_class = getattr(adapter_module, adapter_class_name)
         if not issubclass(adapter_class, AudioAdapter):
             raise SpleeterError(
                 f"{adapter_class_name} is not a valid AudioAdapter class"
             )
         return adapter_class()
```

### Comparing `spleeter-2.3.2/spleeter/audio/convertor.py` & `spleeter-2.4.0/spleeter/audio/convertor.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # coding: utf8
 
 """ This module provides audio data convertion functions. """
 
 # pyright: reportMissingImports=false
 # pylint: disable=import-error
 import numpy as np
-import tensorflow as tf
+import tensorflow as tf  # type: ignore
 
 from ..utils.tensor import from_float32_to_uint8, from_uint8_to_float32
 
 # pylint: enable=import-error
 
 __email__ = "spleeter@deezer.com"
 __author__ = "Deezer Research"
@@ -19,21 +19,21 @@
 
 def to_n_channels(waveform: tf.Tensor, n_channels: int) -> tf.Tensor:
     """
     Convert a waveform to n_channels by removing or duplicating channels if
     needed (in tensorflow).
 
     Parameters:
-        waveform (tensorflow.Tensor):
+        waveform (tf.Tensor):
             Waveform to transform.
         n_channels (int):
             Number of channel to reshape waveform in.
 
     Returns:
-        tensorflow.Tensor:
+        tf.Tensor:
             Reshaped waveform.
     """
     return tf.cond(
         tf.shape(waveform)[1] >= n_channels,
         true_fn=lambda: waveform[:, :n_channels],
         false_fn=lambda: tf.tile(waveform, [1, n_channels])[:, :n_channels],
     )
@@ -41,99 +41,99 @@
 
 def to_stereo(waveform: np.ndarray) -> np.ndarray:
     """
     Convert a waveform to stereo by duplicating if mono, or truncating
     if too many channels.
 
     Parameters:
-        waveform (numpy.ndarray):
+        waveform (np.ndarray):
             a `(N, d)` numpy array.
 
     Returns:
-        numpy.ndarray:
+        np.ndarray:
             A stereo waveform as a `(N, 1)` numpy array.
     """
     if waveform.shape[1] == 1:
         return np.repeat(waveform, 2, axis=-1)
     if waveform.shape[1] > 2:
         return waveform[:, :2]
     return waveform
 
 
 def gain_to_db(tensor: tf.Tensor, espilon: float = 10e-10) -> tf.Tensor:
     """
     Convert from gain to decibel in tensorflow.
 
     Parameters:
-        tensor (tensorflow.Tensor):
+        tensor (tf.Tensor):
             Tensor to convert
         epsilon (float):
             Operation constant.
 
     Returns:
-        tensorflow.Tensor:
+        tf.Tensor:
             Converted tensor.
     """
     return 20.0 / np.log(10) * tf.math.log(tf.maximum(tensor, espilon))
 
 
 def db_to_gain(tensor: tf.Tensor) -> tf.Tensor:
     """
     Convert from decibel to gain in tensorflow.
 
     Parameters:
-        tensor (tensorflow.Tensor):
+        tensor (tf.Tensor):
             Tensor to convert
 
     Returns:
-        tensorflow.Tensor:
+        tf.Tensor:
             Converted tensor.
     """
     return tf.pow(10.0, (tensor / 20.0))
 
 
 def spectrogram_to_db_uint(
     spectrogram: tf.Tensor, db_range: float = 100.0, **kwargs
 ) -> tf.Tensor:
     """
     Encodes given spectrogram into uint8 using decibel scale.
 
     Parameters:
-        spectrogram (tensorflow.Tensor):
+        spectrogram (tf.Tensor):
             Spectrogram to be encoded as TF float tensor.
         db_range (float):
             Range in decibel for encoding.
 
     Returns:
-        tensorflow.Tensor:
+        tf.Tensor:
             Encoded decibel spectrogram as `uint8` tensor.
     """
     db_spectrogram: tf.Tensor = gain_to_db(spectrogram)
     max_db_spectrogram: tf.Tensor = tf.reduce_max(db_spectrogram)
-    db_spectrogram: tf.Tensor = tf.maximum(
+    int_db_spectrogram: tf.Tensor = tf.maximum(
         db_spectrogram, max_db_spectrogram - db_range
     )
-    return from_float32_to_uint8(db_spectrogram, **kwargs)
+    return from_float32_to_uint8(int_db_spectrogram, **kwargs)
 
 
 def db_uint_spectrogram_to_gain(
     db_uint_spectrogram: tf.Tensor, min_db: tf.Tensor, max_db: tf.Tensor
 ) -> tf.Tensor:
     """
     Decode spectrogram from uint8 decibel scale.
 
     Paramters:
-        db_uint_spectrogram (tensorflow.Tensor):
+        db_uint_spectrogram (tf.Tensor):
             Decibel spectrogram to decode.
-        min_db (tensorflow.Tensor):
+        min_db (tf.Tensor):
             Lower bound limit for decoding.
-        max_db (tensorflow.Tensor):
+        max_db (tf.Tensor):
             Upper bound limit for decoding.
 
     Returns:
-        tensorflow.Tensor:
+        tf.Tensor:
             Decoded spectrogram as `float32` tensor.
     """
     db_spectrogram: tf.Tensor = from_uint8_to_float32(
         db_uint_spectrogram, min_db, max_db
     )
     return db_to_gain(db_spectrogram)
```

### Comparing `spleeter-2.3.2/spleeter/audio/ffmpeg.py` & `spleeter-2.4.0/spleeter/audio/ffmpeg.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 #!/usr/bin/env python
 # coding: utf8
 
 """
-    This module provides an AudioAdapter implementation based on FFMPEG
-    process. Such implementation is POSIXish and depends on nothing except
-    standard Python libraries. Thus this implementation is the default one
-    used within this library.
+This module provides an AudioAdapter implementation based on FFMPEG
+process. Such implementation is POSIXish and depends on nothing except
+standard Python libraries. Thus this implementation is the default one
+used within this library.
 """
 
 import datetime as dt
 import os
 import shutil
 from pathlib import Path
 from typing import Dict, Optional, Union
 
 # pyright: reportMissingImports=false
 # pylint: disable=import-error
-import ffmpeg
+import ffmpeg  # type: ignore
 import numpy as np
 
 from .. import SpleeterError
 from ..types import Signal
 from ..utils.logging import logger
 from . import Codec
 from .adapter import AudioAdapter
@@ -63,31 +63,31 @@
 
     def load(
         _,
         path: Union[Path, str],
         offset: Optional[float] = None,
         duration: Optional[float] = None,
         sample_rate: Optional[float] = None,
-        dtype: np.dtype = np.float32,
+        dtype: bytes = b"float32",
     ) -> Signal:
         """
         Loads the audio file denoted by the given path
         and returns it data as a waveform.
 
         Parameters:
             path (Union[Path, str]:
                 Path of the audio file to load data from.
             offset (Optional[float]):
-                Start offset to load from in seconds.
+                (Optional) Start offset to load from in seconds.
             duration (Optional[float]):
-                Duration to load in seconds.
+                (Optional) Duration to load in seconds.
             sample_rate (Optional[float]):
-                Sample rate to load audio with.
-            dtype (numpy.dtype):
-                (Optional) Numpy data type to use, default to `float32`.
+                (Optional) Sample rate to load audio with.
+            dtype (bytes):
+                (Optional) Data type to use, default to `b'float32'`.
 
         Returns:
             Signal:
                 Loaded data a (waveform, sample_rate) tuple.
 
         Raises:
             SpleeterError:
@@ -140,19 +140,19 @@
         """
         Write waveform data to the file denoted by the given path using
         FFMPEG process.
 
         Parameters:
             path (Union[Path, str]):
                 Path like of the audio file to save data in.
-            data (numpy.ndarray):
+            data (np.ndarray):
                 Waveform data to write.
             sample_rate (float):
                 Sample rate to write file in.
-            codec ():
+            codec (Codec):
                 (Optional) Writing codec to use, default to `None`.
             bitrate (str):
                 (Optional) Bitrate of the written audio file, default to
                 `None`.
 
         Raises:
             IOError:
```

### Comparing `spleeter-2.3.2/spleeter/audio/spectrogram.py` & `spleeter-2.4.0/spleeter/audio/spectrogram.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 #!/usr/bin/env python
 # coding: utf8
 
 """ Spectrogram specific data augmentation. """
 
 # pyright: reportMissingImports=false
 # pylint: disable=import-error
-import numpy as np
-import tensorflow as tf
-from tensorflow.signal import hann_window, stft
+import tensorflow as tf  # type: ignore
+from tensorflow.signal import hann_window, stft  # type: ignore
 
 # pylint: enable=import-error
 
 __email__ = "spleeter@deezer.com"
 __author__ = "Deezer Research"
 __license__ = "MIT License"
 
@@ -24,29 +23,29 @@
     window_exponent: float = 1.0,
 ) -> tf.Tensor:
     """
     Compute magnitude / power spectrogram from waveform as a
     `n_samples x n_channels` tensor.
 
     Parameters:
-        waveform (tensorflow.Tensor):
+        waveform (tf.Tensor):
             Input waveform as `(times x number of channels)` tensor.
         frame_length (int):
-            Length of a STFT frame to use.
+            (Optional) Length of a STFT frame to use.
         frame_step (int):
-            HOP between successive frames.
+            (Optional) HOP between successive frames.
         spec_exponent (float):
-            Exponent of the spectrogram (usually 1 for magnitude
-            spectrogram, or 2 for power spectrogram).
+            (Optional) Exponent of the spectrogram (usually 1 for
+            magnitude spectrogram, or 2 for power spectrogram).
         window_exponent (float):
-            Exponent applied to the Hann windowing function (may be
-            useful for making perfect STFT/iSTFT reconstruction).
+            (Optional) Exponent applied to the Hann windowing function
+            (may be useful for making perfect STFT/iSTFT reconstruction).
 
     Returns:
-        tensorflow.Tensor:
+        tf.Tensor:
             Computed magnitude / power spectrogram as a
             `(T x F x n_channels)` tensor.
     """
     stft_tensor: tf.Tensor = tf.transpose(
         stft(
             tf.transpose(waveform),
             frame_length,
@@ -67,23 +66,23 @@
     method: tf.image.ResizeMethod = tf.image.ResizeMethod.BILINEAR,
 ) -> tf.Tensor:
     """
     Time stretch a spectrogram preserving shape in tensorflow. Note that
     this is an approximation in the frequency domain.
 
     Parameters:
-        spectrogram (tensorflow.Tensor):
+        spectrogram (tf.Tensor):
             Input spectrogram to be time stretched as tensor.
         factor (float):
             (Optional) Time stretch factor, must be > 0, default to `1`.
-        method (tensorflow.image.ResizeMethod):
+        method (tf.image.ResizeMethod):
             (Optional) Interpolation method, default to `BILINEAR`.
 
     Returns:
-        tensorflow.Tensor:
+        tf.Tensor:
             Time stretched spectrogram as tensor with same shape.
     """
     T = tf.shape(spectrogram)[0]
     T_ts = tf.cast(tf.cast(T, tf.float32) * factor, tf.int32)[0]
     F = tf.shape(spectrogram)[1]
     ts_spec = tf.image.resize_images(
         spectrogram, [T_ts, F], method=method, align_corners=True
@@ -96,23 +95,25 @@
 ) -> tf.Tensor:
     """
     Time stretch a spectrogram preserving shape with random ratio in
     tensorflow. Applies time_stretch to spectrogram with a random ratio
     drawn uniformly in `[factor_min, factor_max]`.
 
     Parameters:
-        spectrogram (tensorflow.Tensor):
+        spectrogram (tf.Tensor):
             Input spectrogram to be time stretched as tensor.
         factor_min (float):
             (Optional) Min time stretch factor, default to `0.9`.
         factor_max (float):
             (Optional) Max time stretch factor, default to `1.1`.
+        ** kwargs:
+            Time stretch args.
 
     Returns:
-        tensorflow.Tensor:
+        tf.Tensor:
             Randomly time stretched spectrogram as tensor with same shape.
     """
     factor = (
         tf.random_uniform(shape=(1,), seed=0) * (factor_max - factor_min) + factor_min
     )
     return time_stretch(spectrogram, factor=factor, **kwargs)
 
@@ -123,23 +124,23 @@
     method: tf.image.ResizeMethod = tf.image.ResizeMethod.BILINEAR,
 ) -> tf.Tensor:
     """
     Pitch shift a spectrogram preserving shape in tensorflow. Note that
     this is an approximation in the frequency domain.
 
     Parameters:
-        spectrogram (tensorflow.Tensor):
+        spectrogram (tf.Tensor):
             Input spectrogram to be pitch shifted as tensor.
         semitone_shift (float):
             (Optional) Pitch shift in semitone, default to `0.0`.
-        method (tensorflow.image.ResizeMethod):
+        method (tf.image.ResizeMethod):
             (Optional) Interpolation method, default to `BILINEAR`.
 
     Returns:
-        tensorflow.Tensor:
+        tf.Tensor:
             Pitch shifted spectrogram (same shape as spectrogram).
     """
     factor = 2 ** (semitone_shift / 12.0)
     T = tf.shape(spectrogram)[0]
     F = tf.shape(spectrogram)[1]
     F_ps = tf.cast(tf.cast(F, tf.float32) * factor, tf.int32)[0]
     ps_spec = tf.image.resize_images(
@@ -155,22 +156,22 @@
     """
     Pitch shift a spectrogram preserving shape with random ratio in
     tensorflow. Applies pitch_shift to spectrogram with a random shift
     amount (expressed in semitones) drawn uniformly in
     `[shift_min, shift_max]`.
 
     Parameters:
-        spectrogram (tensorflow.Tensor):
+        spectrogram (tf.Tensor):
             Input spectrogram to be pitch shifted as tensor.
         shift_min (float):
             (Optional) Min pitch shift in semitone, default to -1.
         shift_max (float):
             (Optional) Max pitch shift in semitone, default to 1.
 
     Returns:
-        tensorflow.Tensor:
+        tf.Tensor:
             Randomly pitch shifted spectrogram (same shape as spectrogram).
     """
     semitone_shift = (
         tf.random_uniform(shape=(1,), seed=0) * (shift_max - shift_min) + shift_min
     )
     return pitch_shift(spectrogram, semitone_shift=semitone_shift, **kwargs)
```

### Comparing `spleeter-2.3.2/spleeter/dataset.py` & `spleeter-2.4.0/spleeter/dataset.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 #!/usr/bin/env python
 # coding: utf8
 
 """
-    Module for building data preprocessing pipeline using the tensorflow
-    data API. Data preprocessing such as audio loading, spectrogram
-    computation, cropping, feature caching or data augmentation is done
-    using a tensorflow dataset object that output a tuple (input_, output)
-    where:
-
-    -   input is a dictionary with a single key that contains the (batched)
-        mix spectrogram of audio samples
-    -   output is a dictionary of spectrogram of the isolated tracks
-        (ground truth)
+Module for building data preprocessing pipeline using the tensorflow
+data API. Data preprocessing such as audio loading, spectrogram
+computation, cropping, feature caching or data augmentation is done
+using a tensorflow dataset object that output a tuple (input_, output)
+where:
+
+-   input is a dictionary with a single key that contains the (batched)
+    mix spectrogram of audio samples
+-   output is a dictionary of spectrogram of the isolated tracks
+    (ground truth)
 """
 
 import os
 import time
 from os.path import exists
 from os.path import sep as SEPARATOR
-from typing import Any, Dict, Optional
+from typing import Any, Dict, List, Optional, Tuple
 
 # pyright: reportMissingImports=false
 # pylint: disable=import-error
-import tensorflow as tf
+import tensorflow as tf  # type: ignore
 
 from .audio.adapter import AudioAdapter
 from .audio.convertor import db_uint_spectrogram_to_gain, spectrogram_to_db_uint
 from .audio.spectrogram import (
     compute_spectrogram_tf,
     random_pitch_shift,
     random_time_stretch,
@@ -79,17 +79,17 @@
         audio_params,
         audio_adapter,
         audio_path,
         chunk_duration=audio_params.get("chunk_duration", 20.0),
         random_seed=audio_params.get("random_seed", 0),
     )
     return builder.build(
-        audio_params.get("train_csv"),
+        str(audio_params.get("train_csv")),
         cache_directory=audio_params.get("training_cache"),
-        batch_size=audio_params.get("batch_size"),
+        batch_size=audio_params.get("batch_size", 8),
         n_chunks_per_song=audio_params.get("n_chunks_per_song", 2),
         random_data_augmentation=False,
         convert_to_uint=True,
         wait_for_cache=False,
     )
 
 
@@ -111,117 +111,114 @@
         Any:
             Built dataset.
     """
     builder = DatasetBuilder(
         audio_params, audio_adapter, audio_path, chunk_duration=12.0
     )
     return builder.build(
-        audio_params.get("validation_csv"),
-        batch_size=audio_params.get("batch_size"),
+        str(audio_params.get("validation_csv")),
+        batch_size=audio_params.get("batch_size", 8),
         cache_directory=audio_params.get("validation_cache"),
         convert_to_uint=True,
         infinite_generator=False,
         n_chunks_per_song=1,
         # should not perform data augmentation for eval:
         random_data_augmentation=False,
         random_time_crop=False,
         shuffle=False,
     )
 
 
 class InstrumentDatasetBuilder(object):
     """Instrument based filter and mapper provider."""
 
-    def __init__(self, parent, instrument) -> None:
+    def __init__(self, parent: Any, instrument: Any) -> None:
         """
         Default constructor.
 
         Parameters:
-            parent:
+            parent (Any):
                 Parent dataset builder.
-            instrument:
+            instrument (Any):
                 Target instrument.
         """
         self._parent = parent
         self._instrument = instrument
         self._spectrogram_key = f"{instrument}_spectrogram"
         self._min_spectrogram_key = f"min_{instrument}_spectrogram"
         self._max_spectrogram_key = f"max_{instrument}_spectrogram"
 
-    def load_waveform(self, sample):
+    def load_waveform(self, sample: Dict) -> Dict:
         """Load waveform for given sample."""
         return dict(
             sample,
-            **self._parent._audio_adapter.load_tf_waveform(
+            **self._parent._audio_adapter.load_waveform(
                 sample[f"{self._instrument}_path"],
                 offset=sample["start"],
                 duration=self._parent._chunk_duration,
                 sample_rate=self._parent._sample_rate,
                 waveform_name="waveform",
             ),
         )
 
-    def compute_spectrogram(self, sample):
+    def compute_spectrogram(self, sample: Dict) -> Dict:
         """Compute spectrogram of the given sample."""
         return dict(
             sample,
             **{
                 self._spectrogram_key: compute_spectrogram_tf(
                     sample["waveform"],
                     frame_length=self._parent._frame_length,
                     frame_step=self._parent._frame_step,
                     spec_exponent=1.0,
                     window_exponent=1.0,
                 )
             },
         )
 
-    def filter_frequencies(self, sample):
-        """ """
+    def filter_frequencies(self, sample: Dict) -> Dict:
         return dict(
             sample,
             **{
                 self._spectrogram_key: sample[self._spectrogram_key][
                     :, : self._parent._F, :
                 ]
             },
         )
 
-    def convert_to_uint(self, sample):
+    def convert_to_uint(self, sample: Dict) -> Dict:
         """Convert given sample from float to unit."""
         return dict(
             sample,
             **spectrogram_to_db_uint(
                 sample[self._spectrogram_key],
                 tensor_key=self._spectrogram_key,
                 min_key=self._min_spectrogram_key,
                 max_key=self._max_spectrogram_key,
             ),
         )
 
-    def filter_infinity(self, sample):
+    def filter_infinity(self, sample: Dict) -> tf.Tensor:
         """Filter infinity sample."""
         return tf.logical_not(tf.math.is_inf(sample[self._min_spectrogram_key]))
 
-    def convert_to_float32(self, sample):
+    def convert_to_float32(self, sample: Dict) -> Dict:
         """Convert given sample from unit to float."""
         return dict(
             sample,
             **{
                 self._spectrogram_key: db_uint_spectrogram_to_gain(
                     sample[self._spectrogram_key],
                     sample[self._min_spectrogram_key],
                     sample[self._max_spectrogram_key],
                 )
             },
         )
 
-    def time_crop(self, sample):
-        """ """
-
+    def time_crop(self, sample: Dict) -> Dict:
         def start(sample):
             """mid_segment_start"""
             return tf.cast(
                 tf.maximum(
                     tf.shape(sample[self._spectrogram_key])[0] / 2
                     - self._parent._T / 2,
                     0,
@@ -234,122 +231,110 @@
             **{
                 self._spectrogram_key: sample[self._spectrogram_key][
                     start(sample) : start(sample) + self._parent._T, :, :
                 ]
             },
         )
 
-    def filter_shape(self, sample):
+    def filter_shape(self, sample: Dict) -> bool:
         """Filter badly shaped sample."""
         return check_tensor_shape(
             sample[self._spectrogram_key],
             (self._parent._T, self._parent._F, self._parent._n_channels),
         )
 
-    def reshape_spectrogram(self, sample):
+    def reshape_spectrogram(self, sample: Dict) -> Dict:
         """Reshape given sample."""
         return dict(
             sample,
             **{
                 self._spectrogram_key: set_tensor_shape(
                     sample[self._spectrogram_key],
                     (self._parent._T, self._parent._F, self._parent._n_channels),
                 )
             },
         )
 
 
 class DatasetBuilder(object):
-    """
-    TO BE DOCUMENTED.
-    """
-
     MARGIN: float = 0.5
-    """ Margin at beginning and end of songs in seconds. """
+    """Margin at beginning and end of songs in seconds."""
 
     WAIT_PERIOD: int = 60
-    """ Wait period for cache (in seconds). """
+    """Wait period for cache (in seconds)."""
 
     def __init__(
         self,
         audio_params: Dict,
         audio_adapter: AudioAdapter,
         audio_path: str,
         random_seed: int = 0,
         chunk_duration: float = 20.0,
     ) -> None:
         """
         Default constructor.
-
-        NOTE: Probably need for AudioAdapter.
-
-        Parameters:
-            audio_params (Dict):
-                Audio parameters to use.
-            audio_adapter (AudioAdapter):
-                Audio adapter to use.
-            audio_path (str):
-            random_seed (int):
-            chunk_duration (float):
         """
         # Length of segment in frames (if fs=22050 and
         # frame_step=512, then T=512 corresponds to 11.89s)
         self._T = audio_params["T"]
         # Number of frequency bins to be used (should
         # be less than frame_length/2 + 1)
         self._F = audio_params["F"]
         self._sample_rate = audio_params["sample_rate"]
         self._frame_length = audio_params["frame_length"]
         self._frame_step = audio_params["frame_step"]
         self._mix_name = audio_params["mix_name"]
         self._n_channels = audio_params["n_channels"]
         self._instruments = [self._mix_name] + audio_params["instrument_list"]
-        self._instrument_builders = None
+        self._instrument_builders: Optional[List] = None
         self._chunk_duration = chunk_duration
         self._audio_adapter = audio_adapter
         self._audio_params = audio_params
         self._audio_path = audio_path
         self._random_seed = random_seed
 
         self.check_parameters_compatibility()
 
     def check_parameters_compatibility(self):
         if self._frame_length / 2 + 1 < self._F:
             raise ValueError(
-                "F is too large and must be set to at most frame_length/2+1. Decrease F or increase frame_length to fix."
+                "F is too large and must be set to at most frame_length/2+1. "
+                "Decrease F or increase frame_length to fix."
             )
 
         if (
             self._chunk_duration * self._sample_rate - self._frame_length
         ) / self._frame_step < self._T:
             raise ValueError(
-                "T is too large considering STFT parameters and chunk duratoin. Make sure spectrogram time dimension of chunks is larger than T (for instance reducing T or frame_step or increasing chunk duration)."
+                "T is too large considering STFT parameters and chunk duratoin. "
+                "Make sure spectrogram time dimension of chunks is larger than T "
+                "(for instance reducing T or frame_step or increasing chunk duration)."
             )
 
-    def expand_path(self, sample):
+    def expand_path(self, sample: Dict) -> Dict:
         """Expands audio paths for the given sample."""
         return dict(
             sample,
             **{
                 f"{instrument}_path": tf.strings.join(
                     (self._audio_path, sample[f"{instrument}_path"]), SEPARATOR
                 )
                 for instrument in self._instruments
             },
         )
 
-    def filter_error(self, sample):
+    def filter_error(self, sample: Dict) -> tf.Tensor:
         """Filter errored sample."""
         return tf.logical_not(sample["waveform_error"])
 
-    def filter_waveform(self, sample):
+    def filter_waveform(self, sample: Dict) -> Dict:
         """Filter waveform from sample."""
         return {k: v for k, v in sample.items() if not k == "waveform"}
 
-    def harmonize_spectrogram(self, sample):
+    def harmonize_spectrogram(self, sample: Dict) -> Dict:
         """Ensure same size for vocals and mix spectrograms."""
 
         def _reduce(sample):
             return tf.reduce_min(
                 [
                     tf.shape(sample[f"{instrument}_spectrogram"])[0]
                     for instrument in self._instruments
@@ -362,24 +347,24 @@
                 f"{instrument}_spectrogram": sample[f"{instrument}_spectrogram"][
                     : _reduce(sample), :, :
                 ]
                 for instrument in self._instruments
             },
         )
 
-    def filter_short_segments(self, sample):
+    def filter_short_segments(self, sample: Dict) -> tf.Tensor:
         """Filter out too short segment."""
         return tf.reduce_any(
             [
                 tf.shape(sample[f"{instrument}_spectrogram"])[0] >= self._T
                 for instrument in self._instruments
             ]
         )
 
-    def random_time_crop(self, sample):
+    def random_time_crop(self, sample: Dict) -> Dict:
         """Random time crop of 11.88s."""
         return dict(
             sample,
             **sync_apply(
                 {
                     f"{instrument}_spectrogram": sample[f"{instrument}_spectrogram"]
                     for instrument in self._instruments
@@ -388,42 +373,42 @@
                     x,
                     (self._T, len(self._instruments) * self._F, self._n_channels),
                     seed=self._random_seed,
                 ),
             ),
         )
 
-    def random_time_stretch(self, sample):
+    def random_time_stretch(self, sample: Dict) -> Dict:
         """Randomly time stretch the given sample."""
         return dict(
             sample,
             **sync_apply(
                 {
                     f"{instrument}_spectrogram": sample[f"{instrument}_spectrogram"]
                     for instrument in self._instruments
                 },
                 lambda x: random_time_stretch(x, factor_min=0.9, factor_max=1.1),
             ),
         )
 
-    def random_pitch_shift(self, sample):
+    def random_pitch_shift(self, sample: Dict) -> Dict:
         """Randomly pitch shift the given sample."""
         return dict(
             sample,
             **sync_apply(
                 {
                     f"{instrument}_spectrogram": sample[f"{instrument}_spectrogram"]
                     for instrument in self._instruments
                 },
                 lambda x: random_pitch_shift(x, shift_min=-1.0, shift_max=1.0),
                 concat_axis=0,
             ),
         )
 
-    def map_features(self, sample):
+    def map_features(self, sample: Dict) -> Tuple[Dict, Dict]:
         """Select features and annotation of the given sample."""
         input_ = {
             f"{self._mix_name}_spectrogram": sample[f"{self._mix_name}_spectrogram"]
         }
         output = {
             f"{instrument}_spectrogram": sample[f"{instrument}_spectrogram"]
             for instrument in self._audio_params["instrument_list"]
@@ -497,15 +482,15 @@
             for instrument in self._instruments:
                 self._instrument_builders.append(
                     InstrumentDatasetBuilder(self, instrument)
                 )
         for builder in self._instrument_builders:
             yield builder
 
-    def cache(self, dataset: Any, cache: str, wait: bool) -> Any:
+    def cache(self, dataset: Any, cache: Optional[str], wait: bool) -> Any:
         """
         Cache the given dataset if cache is enabled. Eventually waits for
         cache to be available (useful if another process is already
         computing cache) if provided wait flag is `True`.
 
         Parameters:
             dataset (Any):
@@ -537,19 +522,16 @@
         convert_to_uint: bool = True,
         random_data_augmentation: bool = False,
         random_time_crop: bool = True,
         infinite_generator: bool = True,
         cache_directory: Optional[str] = None,
         wait_for_cache: bool = False,
         num_parallel_calls: int = 4,
-        n_chunks_per_song: float = 2,
+        n_chunks_per_song: int = 2,
     ) -> Any:
-        """
-        TO BE DOCUMENTED.
-        """
         dataset = dataset_from_csv(csv_path)
         dataset = self.compute_segments(dataset, n_chunks_per_song)
         # Shuffle data
         if shuffle:
             dataset = dataset.shuffle(
                 buffer_size=200000,
                 seed=self._random_seed,
```

### Comparing `spleeter-2.3.2/spleeter/model/__init__.py` & `spleeter-2.4.0/spleeter/model/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 #!/usr/bin/env python
 # coding: utf8
 
 """ This package provide an estimator builder as well as model functions. """
 
 import importlib
+from typing import Any, Dict, Optional, Tuple
 
 # pyright: reportMissingImports=false
 # pylint: disable=import-error
-import tensorflow as tf
-from tensorflow.signal import hann_window, inverse_stft, stft
+import tensorflow as tf  # type: ignore
+from tensorflow.signal import hann_window, inverse_stft, stft  # type: ignore
 
 from ..utils.tensor import pad_and_partition, pad_and_reshape
 
 # pylint: enable=import-error
 
 
 __email__ = "spleeter@deezer.com"
@@ -25,21 +26,22 @@
 
 def get_model_function(model_type):
     """
     Get tensorflow function of the model to be applied to the input tensor.
     For instance "unet.softmax_unet" will return the softmax_unet function
     in the "unet.py" submodule of the current module (spleeter.model).
 
-    Params:
-    - model_type: str
-    the relative module path to the model function.
+    Parameters:
+        model_type (str):
+            The relative module path to the model function.
 
     Returns:
-    A tensorflow function to be applied to the input tensor to get the
-    multitrack output.
+        Function:
+            A tensorflow function to be applied to the input tensor to get the
+            multitrack output.
     """
     relative_path_to_module = ".".join(model_type.split(".")[:-1])
     model_name = model_type.split(".")[-1]
     main_module = ".".join((__name__, "functions"))
     path_to_module = f"{main_module}.{relative_path_to_module}"
     module = importlib.import_module(path_to_module)
     model_function = getattr(module, model_name)
@@ -74,70 +76,35 @@
         }
         return features
 
     def get_feed_dict(self, features, waveform, audio_id):
         return {features["audio_id"]: audio_id, features["waveform"]: waveform}
 
 
-class SpectralInputProvider(InputProvider):
-    def __init__(self, params):
-        super().__init__(params)
-        self.stft_input_name = "{}_stft".format(self.params["mix_name"])
-
-    @property
-    def input_names(self):
-        return ["audio_id", self.stft_input_name]
-
-    def get_input_dict_placeholders(self):
-        features = {
-            self.stft_input_name: placeholder(
-                tf.complex64,
-                shape=(
-                    None,
-                    self.params["frame_length"] // 2 + 1,
-                    self.params["n_channels"],
-                ),
-                name=self.stft_input_name,
-            ),
-            "audio_id": placeholder(tf.string, name="audio_id"),
-        }
-        return features
-
-    def get_feed_dict(self, features, stft, audio_id):
-        return {features["audio_id"]: audio_id, features[self.stft_input_name]: stft}
-
-
 class InputProviderFactory(object):
     @staticmethod
     def get(params):
-        stft_backend = params["stft_backend"]
-        assert stft_backend in (
-            "tensorflow",
-            "librosa",
-        ), "Unexpected backend {}".format(stft_backend)
-        if stft_backend == "tensorflow":
-            return WaveformInputProvider(params)
-        else:
-            return SpectralInputProvider(params)
+        return WaveformInputProvider(params)
 
 
 class EstimatorSpecBuilder(object):
-    """A builder class that allows to builds a multitrack unet model
+    """
+    A builder class that allows to builds a multitrack unet model
     estimator. The built model estimator has a different behaviour when
     used in a train/eval mode and in predict mode.
 
-    * In train/eval mode:   it takes as input and outputs magnitude spectrogram
-    * In predict mode:      it takes as input and outputs waveform. The whole
-                            separation process is then done in this function
-                            for performance reason: it makes it possible to run
-                            the whole spearation process (including STFT and
-                            inverse STFT) on GPU.
-
-    :Example:
+    * In train/eval mode:
+        It takes as input and outputs magnitude spectrogram
+    * In predict mode:
+        It takes as input and outputs waveform.
+        The whole separation process is then done in this function
+        for performance reason: it makes it possible to run the whole
+        separation process (including STFT and inverse STFT) on GPU.
 
+    Example:
     >>> from spleeter.model import EstimatorSpecBuilder
     >>> builder = EstimatorSpecBuilder()
     >>> builder.build_predict_model()
     >>> builder.build_evaluation_model()
     >>> builder.build_train_model()
 
     >>> from spleeter.model import model_fn
@@ -155,75 +122,81 @@
     ADADELTA = "Adadelta"
     SGD = "SGD"
 
     # Math constants.
     WINDOW_COMPENSATION_FACTOR = 2.0 / 3.0
     EPSILON = 1e-10
 
-    def __init__(self, features, params):
-        """Default constructor. Depending on built model
-        usage, the provided features should be different:
-
-        * In train/eval mode:   features is a dictionary with a
-                                "mix_spectrogram" key, associated to the
-                                mix magnitude spectrogram.
-        * In predict mode:      features is a dictionary with a "waveform"
-                                key, associated to the waveform of the sound
-                                to be separated.
+    def __init__(self, features: Dict, params: Dict) -> None:
+        """
+        Default constructor. Depending on built model usage,
+        the provided features should be different:
 
-        :param features: The input features for the estimator.
-        :param params: Some hyperparameters as a dictionary.
+        * In train/eval mode:
+            Features is a dictionary with a "mix_spectrogram" key,
+            associated to the mix magnitude spectrogram.
+        * In predict mode:
+            Features is a dictionary with a "waveform" key,
+            associated to the waveform of the sound to be separated.
+
+        Parameters:
+            features ():
+                The input features for the estimator.
+            params ():
+                Some hyperparameters as a dictionary.
         """
 
         self._features = features
         self._params = params
         # Get instrument name.
         self._mix_name = params["mix_name"]
         self._instruments = params["instrument_list"]
         # Get STFT/signals parameters
         self._n_channels = params["n_channels"]
         self._T = params["T"]
         self._F = params["F"]
         self._frame_length = params["frame_length"]
         self._frame_step = params["frame_step"]
 
-    def include_stft_computations(self):
-        return self._params["stft_backend"] == "tensorflow"
-
     def _build_model_outputs(self):
-        """Created a batch_sizexTxFxn_channels input tensor containing
-        mix magnitude spectrogram, then an output dict from it according
-        to the selected model in internal parameters.
-
-        :returns: Build output dict.
-        :raise ValueError: If required model_type is not supported.
         """
-
+        Created a batch_sizexTxFxn_channels input tensor containing
+        mix magnitude spectrogram, then an output dict from it
+        according to the selected model in internal parameters.
+
+        Raises:
+            ValueError:
+                If required model_type is not supported.
+        """
         input_tensor = self.spectrogram_feature
         model = self._params.get("model", None)
         if model is not None:
             model_type = model.get("type", self.DEFAULT_MODEL)
         else:
             model_type = self.DEFAULT_MODEL
         try:
             apply_model = get_model_function(model_type)
         except ModuleNotFoundError:
             raise ValueError(f"No model function {model_type} found")
         self._model_outputs = apply_model(
             input_tensor, self._instruments, self._params["model"]["params"]
         )
 
-    def _build_loss(self, labels):
-        """Construct tensorflow loss and metrics
+    def _build_loss(self, labels: Dict) -> Tuple[tf.Tensor, Dict]:
+        """
+        Construct tensorflow loss and metrics
 
-        :param output_dict: dictionary of network outputs (key: instrument
-            name, value: estimated spectrogram of the instrument)
-        :param labels: dictionary of target outputs (key: instrument
-            name, value: ground truth spectrogram of the instrument)
-        :returns: tensorflow (loss, metrics) tuple.
+        Parameters:
+            labels (Dict):
+                Dictionary of target outputs (key: instrument name,
+                value: ground truth spectrogram of the instrument)
+
+        Returns:
+            Tuple[tf.Tensor, Dict]:
+                Tensorflow (loss, metrics) tuple.
         """
         output_dict = self.model_outputs
         loss_type = self._params.get("loss_type", self.L1_MASK)
         if loss_type == self.L1_MASK:
             losses = {
                 name: tf.reduce_mean(tf.abs(output - labels[name]))
                 for name, output in output_dict.items()
@@ -240,20 +213,22 @@
             raise ValueError(f"Unkwnown loss type: {loss_type}")
         loss = tf.reduce_sum(list(losses.values()))
         # Add metrics for monitoring each instrument.
         metrics = {k: tf.compat.v1.metrics.mean(v) for k, v in losses.items()}
         metrics["absolute_difference"] = tf.compat.v1.metrics.mean(loss)
         return loss, metrics
 
-    def _build_optimizer(self):
-        """Builds an optimizer instance from internal parameter values.
-
+    def _build_optimizer(self) -> tf.Tensor:
+        """
+        Builds an optimizer instance from internal parameter values.
         Default to AdamOptimizer if not specified.
 
-        :returns: Optimizer instance from internal configuration.
+        Returns:
+            tf.Tensor:
+                Optimizer instance from internal configuration.
         """
         name = self._params.get("optimizer")
         if name == self.ADADELTA:
             return tf.compat.v1.train.AdadeltaOptimizer()
         rate = self._params["learning_rate"]
         if name == self.SGD:
             return tf.compat.v1.train.GradientDescentOptimizer(rate)
@@ -268,18 +243,18 @@
         return f"{self._mix_name}_stft"
 
     @property
     def spectrogram_name(self):
         return f"{self._mix_name}_spectrogram"
 
     def _build_stft_feature(self):
-        """Compute STFT of waveform and slice the STFT in segment
+        """
+        Compute STFT of waveform and slice the STFT in segment
         with the right length to feed the network.
         """
-
         stft_name = self.stft_name
         spec_name = self.spectrogram_name
 
         if stft_name not in self._features:
             # pad input with a frame of zeros
             waveform = tf.concat(
                 [
@@ -338,19 +313,29 @@
 
     @property
     def masked_stfts(self):
         if not hasattr(self, "_masked_stfts"):
             self._build_masked_stfts()
         return self._masked_stfts
 
-    def _inverse_stft(self, stft_t, time_crop=None):
-        """Inverse and reshape the given STFT
-
-        :param stft_t: input STFT
-        :returns: inverse STFT (waveform)
+    def _inverse_stft(
+        self, stft_t: tf.Tensor, time_crop: Optional[Any] = None
+    ) -> tf.Tensor:
+        """
+        Inverse and reshape the given STFT
+
+        Parameters:
+            stft_t (tf.Tensor):
+                Input STFT.
+            time_crop (Optional[Any]):
+                Time cropping.
+
+        Returns:
+            tf.Tensor:
+                Inverse STFT (waveform).
         """
         inversed = (
             inverse_stft(
                 tf.transpose(stft_t, perm=[2, 0, 1]),
                 self._frame_length,
                 self._frame_step,
                 window_fn=lambda frame_length, dtype: (
@@ -360,23 +345,27 @@
             * self.WINDOW_COMPENSATION_FACTOR
         )
         reshaped = tf.transpose(inversed)
         if time_crop is None:
             time_crop = tf.shape(self._features["waveform"])[0]
         return reshaped[self._frame_length : self._frame_length + time_crop, :]
 
-    def _build_mwf_output_waveform(self):
-        """Perform separation with multichannel Wiener Filtering using Norbert.
-        Note: multichannel Wiener Filtering is not coded in Tensorflow and thus
-        may be quite slow.
+    def _build_mwf_output_waveform(self) -> Dict:
+        """
+        Perform separation with multichannel Wiener Filtering using Norbert.
+
+        Note: multichannel Wiener Filtering is not coded in Tensorflow
+        and thus may be quite slow.
 
-        :returns: dictionary of separated waveforms (key: instrument name,
-            value: estimated waveform of the instrument)
+        Returns:
+            Dict:
+                Dictionary of separated waveforms (key: instrument name,
+                value: estimated waveform of the instrument)
         """
-        import norbert  # pylint: disable=import-error
+        import norbert  # type: ignore # pylint: disable=import-error
 
         output_dict = self.model_outputs
         x = self.stft_feature
         v = tf.stack(
             [
                 pad_and_reshape(
                     output_dict[f"{instrument}_spectrogram"],
@@ -396,21 +385,30 @@
             ),
         )
         return {
             instrument: self._inverse_stft(stft_function[0][:, :, :, k])
             for k, instrument in enumerate(self._instruments)
         }
 
-    def _extend_mask(self, mask):
-        """Extend mask, from reduced number of frequency bin to the number of
-        frequency bin in the STFT.
-
-        :param mask: restricted mask
-        :returns: extended mask
-        :raise ValueError: If invalid mask_extension parameter is set.
+    def _extend_mask(self, mask: tf.Tensor) -> tf.Tensor:
+        """
+        Extend mask, from reduced number of frequency bin to
+        the number of frequency bin in the STFT.
+
+        Parameters:
+            mask (tf.Tensor):
+                Restricted mask.
+
+        Returns:
+            tf.Tensor:
+                Extended mask
+
+        Raises:
+            ValueError:
+                If invalid mask_extension parameter is set.
         """
         extension = self._params["mask_extension"]
         # Extend with average
         # (dispatch according to energy in the processed band)
         if extension == "average":
             extension_row = tf.reduce_mean(mask, axis=2, keepdims=True)
         # Extend with 0
@@ -423,15 +421,14 @@
         n_extra_row = self._frame_length // 2 + 1 - self._F
         extension = tf.tile(extension_row, [1, 1, n_extra_row, 1])
         return tf.concat([mask, extension], axis=2)
 
     def _build_masks(self):
         """
         Compute masks from the output spectrograms of the model.
-        :return:
         """
         output_dict = self.model_outputs
         stft_feature = self.stft_feature
         separation_exponent = self._params["separation_exponent"]
         output_sum = (
             tf.reduce_sum(
                 [e ** separation_exponent for e in output_dict.values()], axis=0
@@ -462,111 +459,126 @@
     def _build_masked_stfts(self):
         input_stft = self.stft_feature
         out = {}
         for instrument, mask in self.masks.items():
             out[instrument] = tf.cast(mask, dtype=tf.complex64) * input_stft
         self._masked_stfts = out
 
-    def _build_manual_output_waveform(self, masked_stft):
-        """Perform ratio mask separation
-
-        :param output_dict: dictionary of estimated spectrogram (key: instrument
-            name, value: estimated spectrogram of the instrument)
-        :returns: dictionary of separated waveforms (key: instrument name,
-            value: estimated waveform of the instrument)
+    def _build_manual_output_waveform(self, masked_stft: Dict) -> Dict:
         """
+        Perform ratio mask separation
 
+        Parameters:
+            masked_stft (Dict):
+                Dictionary of estimated spectrogram (key: instrument name,
+                value: estimated spectrogram of the instrument).
+
+        Returns:
+            Dict:
+                Dictionary of separated waveforms (key: instrument name,
+                value: estimated waveform of the instrument).
+        """
         output_waveform = {}
         for instrument, stft_data in masked_stft.items():
             output_waveform[instrument] = self._inverse_stft(stft_data)
         return output_waveform
 
-    def _build_output_waveform(self, masked_stft):
-        """Build output waveform from given output dict in order to be used in
-        prediction context. Regarding of the configuration building method will
-        be using MWF.
-
-        :returns: Built output waveform.
+    def _build_output_waveform(self, masked_stft: Dict) -> Dict:
+        """
+        Build output waveform from given output dict in order
+        to be used in prediction context. The configuration
+        building method will be using MWF.
+
+        masked_stft (Dict):
+                Dictionary of estimated spectrogram (key: instrument name,
+                value: estimated spectrogram of the instrument).
+
+        Returns:
+            Dict:
+                Built output waveform.
         """
 
         if self._params.get("MWF", False):
             output_waveform = self._build_mwf_output_waveform()
         else:
             output_waveform = self._build_manual_output_waveform(masked_stft)
         return output_waveform
 
     def _build_outputs(self):
-        if self.include_stft_computations():
-            self._outputs = self._build_output_waveform(self.masked_stfts)
-        else:
-            self._outputs = self.masked_stfts
+        self._outputs = self._build_output_waveform(self.masked_stfts)
 
         if "audio_id" in self._features:
             self._outputs["audio_id"] = self._features["audio_id"]
 
-    def build_predict_model(self):
-        """Builder interface for creating model instance that aims to perform
+    def build_predict_model(self) -> tf.Tensor:
+        """
+        Builder interface for creating model instance that aims to perform
         prediction / inference over given track. The output of such estimator
-        will be a dictionary with a "<instrument>" key per separated instrument
-        , associated to the estimated separated waveform of the instrument.
+        will be a dictionary with a "<instrument>" key per separated instrument,
+        associated to the estimated separated waveform of the instrument.
 
-        :returns: An estimator for performing prediction.
+        Returns:
+            tf.Tensor:
+                An estimator for performing prediction.
         """
 
         return tf.estimator.EstimatorSpec(
             tf.estimator.ModeKeys.PREDICT, predictions=self.outputs
         )
 
-    def build_evaluation_model(self, labels):
-        """Builder interface for creating model instance that aims to perform
-        model evaluation. The output of such estimator will be a dictionary
-        with a key "<instrument>_spectrogram" per separated instrument,
-        associated to the estimated separated instrument magnitude spectrogram.
-
-        :param labels: Model labels.
-        :returns: An estimator for performing model evaluation.
+    def build_evaluation_model(self, labels: Dict) -> tf.Tensor:
+        """
+        Builder interface for creating model instance that aims
+        to perform model evaluation. The output of such estimator
+        will be a dictionary with a key "<instrument>_spectrogram"
+        per separated instrument, associated to the estimated
+        separated instrument magnitude spectrogram.
+
+        Parameters:
+            labels (Dict):
+                Model labels.
+
+        Returns:
+            tf.Tensor:
+                An estimator for performing model evaluation.
         """
         loss, metrics = self._build_loss(labels)
         return tf.estimator.EstimatorSpec(
             tf.estimator.ModeKeys.EVAL, loss=loss, eval_metric_ops=metrics
         )
 
-    def build_train_model(self, labels):
-        """Builder interface for creating model instance that aims to perform
+    def build_train_model(self, labels: Dict) -> tf.Tensor:
+        """
+        Builder interface for creating model instance that aims to perform
         model training. The output of such estimator will be a dictionary
         with a key "<instrument>_spectrogram" per separated instrument,
         associated to the estimated separated instrument magnitude spectrogram.
 
-        :param labels: Model labels.
-        :returns: An estimator for performing model training.
+        Parameters:
+            labels (Dict):
+                Model labels.
+
+        Returns:
+            tf.Tensor:
+                An estimator for performing model training.
         """
         loss, metrics = self._build_loss(labels)
         optimizer = self._build_optimizer()
         train_operation = optimizer.minimize(
             loss=loss, global_step=tf.compat.v1.train.get_global_step()
         )
         return tf.estimator.EstimatorSpec(
             mode=tf.estimator.ModeKeys.TRAIN,
             loss=loss,
             train_op=train_operation,
             eval_metric_ops=metrics,
         )
 
 
-def model_fn(features, labels, mode, params, config):
-    """
-
-    :param features:
-    :param labels:
-    :param mode: Estimator mode.
-    :param params:
-    :param config: TF configuration (not used).
-    :returns: Built EstimatorSpec.
-    :raise ValueError: If estimator mode is not supported.
-    """
+def model_fn(features, labels, mode, params):
     builder = EstimatorSpecBuilder(features, params)
     if mode == tf.estimator.ModeKeys.PREDICT:
         return builder.build_predict_model()
     elif mode == tf.estimator.ModeKeys.EVAL:
         return builder.build_evaluation_model(labels)
     elif mode == tf.estimator.ModeKeys.TRAIN:
         return builder.build_train_model(labels)
```

### Comparing `spleeter-2.3.2/spleeter/model/functions/__init__.py` & `spleeter-2.4.0/spleeter/model/functions/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 """ This package provide model functions. """
 
 from typing import Callable, Dict, Iterable, Optional
 
 # pyright: reportMissingImports=false
 # pylint: disable=import-error
-import tensorflow as tf
+import tensorflow as tf  # type: ignore
 
 # pylint: enable=import-error
 
 __email__ = "spleeter@deezer.com"
 __author__ = "Deezer Research"
 __license__ = "MIT License"
 
@@ -22,25 +22,26 @@
     instruments: Iterable[str],
     params: Optional[Dict] = None,
 ) -> Dict:
     """
     Apply given function to the input tensor.
 
     Parameters:
-        function:
+        function (Callable):
             Function to be applied to tensor.
-        input_tensor (tensorflow.Tensor):
+        input_tensor (tf.Tensor):
             Tensor to apply blstm to.
         instruments (Iterable[str]):
             Iterable that provides a collection of instruments.
-        params:
+        params (Optional[Dict]):
             (Optional) dict of BLSTM parameters.
 
     Returns:
-        Created output tensor dict.
+        Dict:
+            Created output tensor dict.
     """
     output_dict: Dict = {}
     for instrument in instruments:
         out_name = f"{instrument}_spectrogram"
         output_dict[out_name] = function(
             input_tensor, output_name=out_name, params=params or {}
         )
```

### Comparing `spleeter-2.3.2/spleeter/model/functions/blstm.py` & `spleeter-2.4.0/spleeter/model/functions/blstm.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 #!/usr/bin/env python
 # coding: utf8
 
 """
-    This system (UHL1) uses a bi-directional LSTM network as described in :
+This system (UHL1) uses a bi-directional LSTM network as described in :
 
-    `S. Uhlich, M. Porcu, F. Giron, M. Enenkl, T. Kemp, N. Takahashi and
-    Y. Mitsufuji.
+`S. Uhlich, M. Porcu, F. Giron, M. Enenkl, T. Kemp, N. Takahashi and
+Y. Mitsufuji.
 
-    "Improving music source separation based on deep neural networks through
-    data augmentation and network blending", Proc. ICASSP, 2017.`
+"Improving music source separation based on deep neural networks through
+data augmentation and network blending", Proc. ICASSP, 2017.`
 
-    It has three BLSTM layers, each having 500 cells.  For each instrument,
-    a network is trained which predicts the target instrument amplitude from
-    the mixture amplitude in the STFT domain (frame size: 4096, hop size:
-    1024). The raw output of each network is then combined by a multichannel
-    Wiener filter. The network is trained on musdb where we split train into
-    train_train and train_valid with 86 and 14 songs, respectively. The
-    validation set is used to perform early stopping and hyperparameter
-    selection (LSTM layer dropout rate, regularization strength).
+It has three BLSTM layers, each having 500 cells.  For each instrument,
+a network is trained which predicts the target instrument amplitude from
+the mixture amplitude in the STFT domain (frame size: 4096, hop size:
+1024). The raw output of each network is then combined by a multichannel
+Wiener filter. The network is trained on musdb where we split train into
+train_train and train_valid with 86 and 14 songs, respectively. The
+validation set is used to perform early stopping and hyperparameter
+selection (LSTM layer dropout rate, regularization strength).
 """
 
 from typing import Dict, Optional
 
 # pyright: reportMissingImports=false
 # pylint: disable=import-error
-import tensorflow as tf
-from tensorflow.compat.v1.keras.initializers import he_uniform
-from tensorflow.compat.v1.keras.layers import CuDNNLSTM
-from tensorflow.keras.layers import (
+import tensorflow as tf  # type: ignore
+from tensorflow.compat.v1.keras.initializers import he_uniform  # type: ignore
+from tensorflow.compat.v1.keras.layers import CuDNNLSTM  # type: ignore
+from tensorflow.keras.layers import (  # type: ignore
     Bidirectional,
     Dense,
     Flatten,
     Reshape,
     TimeDistributed,
 )
 
@@ -47,23 +47,23 @@
 def apply_blstm(
     input_tensor: tf.Tensor, output_name: str = "output", params: Optional[Dict] = None
 ) -> tf.Tensor:
     """
     Apply BLSTM to the given input_tensor.
 
     Parameters:
-        input_tensor (tensorflow.Tensor):
+        input_tensor (tf.Tensor):
             Input of the model.
         output_name (str):
             (Optional) name of the output, default to 'output'.
         params (Optional[Dict]):
             (Optional) dict of BLSTM parameters.
 
     Returns:
-        tensorflow.Tensor:
+        tf.Tensor:
             Output tensor.
     """
     if params is None:
         params = {}
     units: int = params.get("lstm_units", 250)
     kernel_initializer = he_uniform(seed=50)
     flatten_input = TimeDistributed(Flatten())((input_tensor))
```

### Comparing `spleeter-2.3.2/spleeter/model/functions/unet.py` & `spleeter-2.4.0/spleeter/model/functions/unet.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 #!/usr/bin/env python
 # coding: utf8
 
 """
-    This module contains building functions for U-net source
-    separation models in a similar way as in A. Jansson et al. :
+This module contains building functions for U-net source
+separation models in a similar way as in A. Jansson et al. :
 
-    "Singing voice separation with deep u-net convolutional networks",
-    ISMIR 2017
+"Singing voice separation with deep u-net convolutional networks",
+ISMIR 2017
 
-    Each instrument is modeled by a single U-net
-    convolutional / deconvolutional network that take a mix spectrogram
-    as input and the estimated sound spectrogram as output.
+Each instrument is modeled by a single U-net
+convolutional / deconvolutional network that take a mix spectrogram
+as input and the estimated sound spectrogram as output.
 """
 
 from functools import partial
 from typing import Any, Dict, Iterable, Optional
 
 # pyright: reportMissingImports=false
 # pylint: disable=import-error
-import tensorflow as tf
-from tensorflow.compat.v1 import logging
-from tensorflow.compat.v1.keras.initializers import he_uniform
-from tensorflow.keras.layers import (
+import tensorflow as tf  # type: ignore
+from tensorflow.compat.v1 import logging  # type: ignore
+from tensorflow.compat.v1.keras.initializers import he_uniform  # type: ignore
+from tensorflow.keras.layers import (  # type: ignore
     ELU,
     BatchNormalization,
     Concatenate,
     Conv2D,
     Conv2DTranspose,
     Dropout,
     LeakyReLU,
@@ -41,65 +41,71 @@
 __email__ = "spleeter@deezer.com"
 __author__ = "Deezer Research"
 __license__ = "MIT License"
 
 
 def _get_conv_activation_layer(params: Dict) -> Any:
     """
-    > To be documented.
-
     Parameters:
         params (Dict):
+            Model parameters.
 
     Returns:
         Any:
             Required Activation function.
     """
-    conv_activation: str = params.get("conv_activation")
+    conv_activation: str = str(params.get("conv_activation"))
     if conv_activation == "ReLU":
         return ReLU()
     elif conv_activation == "ELU":
         return ELU()
     return LeakyReLU(0.2)
 
 
 def _get_deconv_activation_layer(params: Dict) -> Any:
     """
-    > To be documented.
-
     Parameters:
         params (Dict):
+            Model parameters.
 
     Returns:
         Any:
             Required Activation function.
     """
-    deconv_activation: str = params.get("deconv_activation")
+    deconv_activation: str = str(params.get("deconv_activation"))
     if deconv_activation == "LeakyReLU":
         return LeakyReLU(0.2)
     elif deconv_activation == "ELU":
         return ELU()
     return ReLU()
 
 
 def apply_unet(
     input_tensor: tf.Tensor,
     output_name: str = "output",
-    params: Optional[Dict] = None,
+    params: Dict = {},
     output_mask_logit: bool = False,
-) -> Any:
+) -> tf.Tensor:
     """
     Apply a convolutionnal U-net to model a single instrument (one U-net
     is used for each instrument).
 
     Parameters:
-        input_tensor (tensorflow.Tensor):
+        input_tensor (tf.Tensor):
+            Input of the model.
         output_name (str):
-        params (Optional[Dict]):
+            (Optional) name of the output, default to 'output'.
+        params (Dict):
+            (Optional) dict of BLSTM parameters.
         output_mask_logit (bool):
+            (Optional) Sigmoid or logit?
+
+    Returns:
+        tf.Tensor:
+            Output tensor.
     """
     logging.info(f"Apply unet for {output_name}")
     conv_n_filters = params.get("conv_n_filters", [16, 32, 64, 128, 256, 512])
     conv_activation_layer = _get_conv_activation_layer(params)
     deconv_activation_layer = _get_deconv_activation_layer(params)
     kernel_initializer = he_uniform(seed=50)
     conv2d_factory = partial(
@@ -194,25 +200,25 @@
     input_tensor: tf.Tensor, instruments: Iterable[str], params: Optional[Dict] = None
 ) -> Dict:
     """Model function applier."""
     return apply(apply_unet, input_tensor, instruments, params)
 
 
 def softmax_unet(
-    input_tensor: tf.Tensor, instruments: Iterable[str], params: Optional[Dict] = None
+    input_tensor: tf.Tensor, instruments: Iterable[str], params: Dict = {}
 ) -> Dict:
     """
     Apply softmax to multitrack unet in order to have mask suming to one.
 
     Parameters:
-        input_tensor (tensorflow.Tensor):
+        input_tensor (tf.Tensor):
             Tensor to apply blstm to.
         instruments (Iterable[str]):
             Iterable that provides a collection of instruments.
-        params (Optional[Dict]):
+        params (Dict):
             (Optional) dict of BLSTM parameters.
 
     Returns:
         Dict:
             Created output tensor dict.
     """
     logit_mask_list = []
```

### Comparing `spleeter-2.3.2/spleeter/model/provider/__init__.py` & `spleeter-2.4.0/spleeter/model/provider/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 #!/usr/bin/env python
 # coding: utf8
 
 """
-    This package provides tools for downloading model from network
-    using remote storage abstraction.
+This package provides tools for downloading model from network
+using remote storage abstraction.
 
-    Examples:
-
-    ```python
-    >>> provider = MyProviderImplementation()
-    >>> provider.get('/path/to/local/storage', params)
-    ```
+Example:
+```python
+>>> provider = MyProviderImplementation()
+>>> provider.get('/path/to/local/storage', params)
+```
 """
 
 from abc import ABC, abstractmethod
 from os import environ, makedirs
 from os.path import exists, isabs, join, sep
 
 __email__ = "spleeter@deezer.com"
@@ -64,14 +63,18 @@
         Parameters:
             model_directory (str):
                 Expected model_directory to be available.
 
         Raises:
             IOError:
                 If model can not be retrieved.
+
+        Returns:
+            str:
+                Available model directory.
         """
         # Expend model directory if needed.
         if not isabs(model_directory):
             model_directory = join(self.DEFAULT_MODEL_PATH, model_directory)
         # Download it if not exists.
         model_probe: str = join(model_directory, self.MODEL_PROBE_PATH)
         if not exists(model_probe):
```

### Comparing `spleeter-2.3.2/spleeter/model/provider/github.py` & `spleeter-2.4.0/spleeter/model/provider/github.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 #!/usr/bin/env python
 # coding: utf8
 
 """
-    A ModelProvider backed by Github Release feature.
+A ModelProvider backed by Github Release feature.
 
-    Examples:
+Examples:
 
-    ```python
-    >>> from spleeter.model.provider import github
-    >>> provider = github.GithubModelProvider(
-            'github.com',
-            'Deezer/spleeter',
-            'latest')
-    >>> provider.download('2stems', '/path/to/local/storage')
-    ```
+```python
+>>> from spleeter.model.provider import github
+>>> provider = github.GithubModelProvider(
+        'github.com',
+        'Deezer/spleeter',
+        'latest')
+>>> provider.download('2stems', '/path/to/local/storage')
+```
 """
 
 import hashlib
 import os
 import tarfile
 from os import environ
 from tempfile import NamedTemporaryFile
@@ -34,18 +34,24 @@
 
 __email__ = "spleeter@deezer.com"
 __author__ = "Deezer Research"
 __license__ = "MIT License"
 
 
 def compute_file_checksum(path):
-    """Computes given path file sha256.
+    """
+    Computes given path file sha256.
 
-    :param path: Path of the file to compute checksum for.
-    :returns: File checksum.
+    Parameters:
+        path (str):
+            Path of the file to compute checksum for.
+
+    Returns:
+        str:
+            File checksum.
     """
     sha256 = hashlib.sha256()
     with open(path, "rb") as stream:
         for chunk in iter(lambda: stream.read(4096), b""):
             sha256.update(chunk)
     return sha256.hexdigest()
 
@@ -72,15 +78,15 @@
                 Release name to get models from.
         """
         self._host: str = host
         self._repository: str = repository
         self._release: str = release
 
     @classmethod
-    def from_environ(cls: type) -> "GithubModelProvider":
+    def from_environ(cls) -> "GithubModelProvider":
         """
         Factory method that creates provider from envvars.
 
         Returns:
             GithubModelProvider:
                 Created instance.
         """
@@ -93,14 +99,15 @@
     def checksum(self, name: str) -> str:
         """
         Downloads and returns reference checksum for the given model name.
 
         Parameters:
             name (str):
                 Name of the model to get checksum for.
+
         Returns:
             str:
                 Checksum of the required model.
 
         Raises:
             ValueError:
                 If the given model name is not indexed.
```

### Comparing `spleeter-2.3.2/spleeter/options.py` & `spleeter-2.4.0/spleeter/options.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,148 +1,133 @@
 #!/usr/bin/env python
 # coding: utf8
 
-""" This modules provides spleeter command as well as CLI parsing methods. """
+"""This modules provides spleeter command as well as CLI parsing methods."""
 
 from os.path import join
 from tempfile import gettempdir
 
 from typer import Argument, Exit, Option, echo
-from typer.models import ArgumentInfo, OptionInfo
+from typer.models import List, Optional
 
-from .audio import Codec, STFTBackend
+from .audio import Codec
 
 __email__ = "spleeter@deezer.com"
 __author__ = "Deezer Research"
 __license__ = "MIT License"
 
-AudioInputArgument: ArgumentInfo = Argument(
+AudioInputArgument: List[str] = Argument(
     ...,
     help="List of input audio file path",
     exists=True,
     file_okay=True,
     dir_okay=False,
     readable=True,
     resolve_path=True,
 )
 
-AudioInputOption: OptionInfo = Option(
+AudioInputOption: Optional[str] = Option(
     None, "--inputs", "-i", help="(DEPRECATED) placeholder for deprecated input option"
 )
 
-AudioAdapterOption: OptionInfo = Option(
+AudioAdapterOption: str = Option(
     "spleeter.audio.ffmpeg.FFMPEGProcessAudioAdapter",
     "--adapter",
     "-a",
     help="Name of the audio adapter to use for audio I/O",
 )
 
-AudioOutputOption: OptionInfo = Option(
+AudioOutputOption: str = Option(
     join(gettempdir(), "separated_audio"),
     "--output_path",
     "-o",
     help="Path of the output directory to write audio files in",
 )
 
-AudioOffsetOption: OptionInfo = Option(
+AudioOffsetOption: float = Option(
     0.0, "--offset", "-s", help="Set the starting offset to separate audio from"
 )
 
-AudioDurationOption: OptionInfo = Option(
+AudioDurationOption: float = Option(
     600.0,
     "--duration",
     "-d",
     help=(
         "Set a maximum duration for processing audio "
         "(only separate offset + duration first seconds of "
         "the input file)"
     ),
 )
 
-AudioSTFTBackendOption: OptionInfo = Option(
-    STFTBackend.AUTO,
-    "--stft-backend",
-    "-B",
-    case_sensitive=False,
-    help=(
-        "Who should be in charge of computing the stfts. Librosa is faster "
-        'than tensorflow on CPU and uses  less memory. "auto" will use '
-        "tensorflow when GPU acceleration is available and librosa when not"
-    ),
-)
-
-AudioCodecOption: OptionInfo = Option(
+AudioCodecOption: Codec = Option(
     Codec.WAV, "--codec", "-c", help="Audio codec to be used for the separated output"
 )
 
-AudioBitrateOption: OptionInfo = Option(
+AudioBitrateOption: str = Option(
     "128k", "--bitrate", "-b", help="Audio bitrate to be used for the separated output"
 )
 
-FilenameFormatOption: OptionInfo = Option(
+FilenameFormatOption: str = Option(
     "{filename}/{instrument}.{codec}",
     "--filename_format",
     "-f",
     help=(
         "Template string that will be formatted to generated"
         "output filename. Such template should be Python formattable"
         "string, and could use {filename}, {instrument}, and {codec}"
         "variables"
     ),
 )
 
-ModelParametersOption: OptionInfo = Option(
+ModelParametersOption: str = Option(
     "spleeter:2stems",
     "--params_filename",
     "-p",
     help="JSON filename that contains params",
 )
 
 
-MWFOption: OptionInfo = Option(
+MWFOption: bool = Option(
     False, "--mwf", help="Whether to use multichannel Wiener filtering for separation"
 )
 
-MUSDBDirectoryOption: OptionInfo = Option(
+MUSDBDirectoryOption: str = Option(
     ...,
     "--mus_dir",
     exists=True,
     dir_okay=True,
     file_okay=False,
     readable=True,
     resolve_path=True,
     help="Path to musDB dataset directory",
 )
 
-TrainingDataDirectoryOption: OptionInfo = Option(
+TrainingDataDirectoryOption: str = Option(
     ...,
     "--data",
     "-d",
     exists=True,
     dir_okay=True,
     file_okay=False,
     readable=True,
     resolve_path=True,
     help="Path of the folder containing audio data for training",
 )
 
-VerboseOption: OptionInfo = Option(False, "--verbose", help="Enable verbose logs")
+VerboseOption: bool = Option(False, "--verbose", help="Enable verbose logs")
 
 
 def version_callback(value: bool):
     if value:
-        try:
-            from importlib.metadata import version
-        except ImportError:
-            from importlib_metadata import version
+        from importlib.metadata import version
 
         echo(f"Spleeter Version: {version('spleeter')}")
         raise Exit()
 
 
-VersionOption: OptionInfo = Option(
+VersionOption: bool = Option(
     None,
     "--version",
     callback=version_callback,
     is_eager=True,
     help="Return Spleeter version",
 )
```

### Comparing `spleeter-2.3.2/spleeter/resources/2stems-16kHz.json` & `spleeter-2.4.0/spleeter/resources/2stems-16kHz.json`

 * *Files identical despite different names*

### Comparing `spleeter-2.3.2/spleeter/resources/2stems.json` & `spleeter-2.4.0/spleeter/resources/2stems.json`

 * *Files identical despite different names*

### Comparing `spleeter-2.3.2/spleeter/resources/4stems-16kHz.json` & `spleeter-2.4.0/spleeter/resources/4stems-16kHz.json`

 * *Files identical despite different names*

### Comparing `spleeter-2.3.2/spleeter/resources/4stems.json` & `spleeter-2.4.0/spleeter/resources/4stems.json`

 * *Files identical despite different names*

### Comparing `spleeter-2.3.2/spleeter/resources/5stems-16kHz.json` & `spleeter-2.4.0/spleeter/resources/5stems-16kHz.json`

 * *Files identical despite different names*

### Comparing `spleeter-2.3.2/spleeter/resources/5stems.json` & `spleeter-2.4.0/spleeter/resources/5stems.json`

 * *Files identical despite different names*

### Comparing `spleeter-2.3.2/spleeter/resources/musdb.json` & `spleeter-2.4.0/spleeter/resources/musdb.json`

 * *Files identical despite different names*

### Comparing `spleeter-2.3.2/spleeter/separator.py` & `spleeter-2.4.0/spleeter/separator.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,40 +1,36 @@
 #!/usr/bin/env python
 # coding: utf8
 
 """
-    Module that provides a class wrapper for source separation.
+Module that provides a class wrapper for source separation.
 
-    Examples:
+Examples:
 
-    ```python
-    >>> from spleeter.separator import Separator
-    >>> separator = Separator('spleeter:2stems')
-    >>> separator.separate(waveform, lambda instrument, data: ...)
-    >>> separator.separate_to_file(...)
-    ```
+```python
+>>> from spleeter.separator import Separator
+>>> separator = Separator('spleeter:2stems')
+>>> separator.separate(waveform, lambda instrument, data: ...)
+>>> separator.separate_to_file(...)
+```
 """
 
 import atexit
 import os
 from multiprocessing import Pool
 from os.path import basename, dirname, join, splitext
-from typing import Dict, Generator, Optional
+from typing import Any, Dict, Generator, List, Optional
 
 # pyright: reportMissingImports=false
 # pylint: disable=import-error
 import numpy as np
-import tensorflow as tf
-from librosa.core import istft, stft
-from scipy.signal.windows import hann
-
-from spleeter.model.provider import ModelProvider
+import tensorflow as tf  # type: ignore
 
 from . import SpleeterError
-from .audio import Codec, STFTBackend
+from .audio import Codec
 from .audio.adapter import AudioAdapter
 from .audio.convertor import to_stereo
 from .model import EstimatorSpecBuilder, InputProviderFactory, model_fn
 from .model.provider import ModelProvider
 from .types import AudioDescriptor
 from .utils.configuration import load_configuration
 
@@ -64,23 +60,27 @@
         """Generation process."""
         buffer = self._current_data
         while buffer:
             yield buffer
             buffer = self._current_data
 
 
-def create_estimator(params, MWF):
+def create_estimator(params: Dict, MWF: bool) -> tf.Tensor:
     """
     Initialize tensorflow estimator that will perform separation
 
-    Params:
-    - params: a dictionary of parameters for building the model
+    Parameters:
+        params (Dict):
+            A dictionary of parameters for building the model
+        MWF (bool):
+            Wiener filter enabled?
 
     Returns:
-        a tensorflow estimator
+        tf.Tensor:
+            A tensorflow estimator
     """
     # Load model.
     provider: ModelProvider = ModelProvider.default()
     params["model_dir"] = provider.get(params["model_dir"])
     params["MWF"] = MWF
     # Setup config
     session_config = tf.compat.v1.ConfigProto()
@@ -96,42 +96,42 @@
 class Separator(object):
     """A wrapper class for performing separation."""
 
     def __init__(
         self,
         params_descriptor: str,
         MWF: bool = False,
-        stft_backend: STFTBackend = STFTBackend.AUTO,
         multiprocess: bool = True,
     ) -> None:
         """
         Default constructor.
 
         Parameters:
             params_descriptor (str):
                 Descriptor for TF params to be used.
             MWF (bool):
                 (Optional) `True` if MWF should be used, `False` otherwise.
+            multiprocess (bool):
+                (Optional) Enable multi-processing.
         """
         self._params = load_configuration(params_descriptor)
         self._sample_rate = self._params["sample_rate"]
         self._MWF = MWF
         self._tf_graph = tf.Graph()
-        self._prediction_generator = None
+        self._prediction_generator: Optional[Generator] = None
         self._input_provider = None
         self._builder = None
         self._features = None
         self._session = None
         if multiprocess:
-            self._pool = Pool()
+            self._pool: Optional[Any] = Pool()
             atexit.register(self._pool.close)
         else:
             self._pool = None
-        self._tasks = []
-        self._params["stft_backend"] = STFTBackend.resolve(stft_backend)
+        self._tasks: List = []
         self._data_generator = DataGenerator()
 
     def _get_prediction_generator(self) -> Generator:
         """
         Lazy loading access method for internal prediction generator
         returned by the predict method of a tensorflow estimator.
 
@@ -156,68 +156,21 @@
 
     def join(self, timeout: int = 200) -> None:
         """
         Wait for all pending tasks to be finished.
 
         Parameters:
             timeout (int):
-                (Optional) task waiting timeout.
+                (Optional) Task waiting timeout.
         """
         while len(self._tasks) > 0:
             task = self._tasks.pop()
             task.get()
             task.wait(timeout=timeout)
 
-    def _stft(
-        self, data: np.ndarray, inverse: bool = False, length: Optional[int] = None
-    ) -> np.ndarray:
-        """
-        Single entrypoint for both stft and istft. This computes stft and
-        istft with librosa on stereo data. The two channels are processed
-        separately and are concatenated together in the result. The
-        expected input formats are: (n_samples, 2) for stft and (T, F, 2)
-        for istft.
-
-        Parameters:
-            data (numpy.array):
-                Array with either the waveform or the complex spectrogram
-                depending on the parameter inverse
-            inverse (bool):
-                (Optional) Should a stft or an istft be computed.
-            length (Optional[int]):
-
-        Returns:
-            numpy.ndarray:
-                Stereo data as numpy array for the transform. The channels
-                are stored in the last dimension.
-        """
-        assert not (inverse and length is None)
-        data = np.asfortranarray(data)
-        N = self._params["frame_length"]
-        H = self._params["frame_step"]
-        win = hann(N, sym=False)
-        fstft = istft if inverse else stft
-        win_len_arg = {"win_length": None, "length": None} if inverse else {"n_fft": N}
-        n_channels = data.shape[-1]
-        out = []
-        for c in range(n_channels):
-            d = (
-                np.concatenate((np.zeros((N,)), data[:, c], np.zeros((N,))))
-                if not inverse
-                else data[:, :, c].T
-            )
-            s = fstft(d, hop_length=H, window=win, center=False, **win_len_arg)
-            if inverse:
-                s = s[N : N + length]
-            s = np.expand_dims(s.T, 2 - inverse)
-            out.append(s)
-        if len(out) == 1:
-            return out[0]
-        return np.concatenate(out, axis=2 - inverse)
-
     def _get_input_provider(self):
         if self._input_provider is None:
             self._input_provider = InputProviderFactory.get(self._params)
         return self._input_provider
 
     def _get_features(self):
         if self._features is None:
@@ -236,63 +189,30 @@
             provider = ModelProvider.default()
             model_directory: str = provider.get(self._params["model_dir"])
             latest_checkpoint = tf.train.latest_checkpoint(model_directory)
             self._session = tf.compat.v1.Session()
             saver.restore(self._session, latest_checkpoint)
         return self._session
 
-    def _separate_librosa(
-        self, waveform: np.ndarray, audio_descriptor: AudioDescriptor
-    ) -> Dict:
-        """
-        Performs separation with librosa backend for STFT.
-
-        Parameters:
-            waveform (numpy.ndarray):
-                Waveform to be separated (as a numpy array)
-            audio_descriptor (AudioDescriptor):
-        """
-        with self._tf_graph.as_default():
-            out = {}
-            features = self._get_features()
-            # TODO: fix the logic, build sometimes return,
-            #       sometimes set attribute.
-            outputs = self._get_builder().outputs
-            stft = self._stft(waveform)
-            if stft.shape[-1] == 1:
-                stft = np.concatenate([stft, stft], axis=-1)
-            elif stft.shape[-1] > 2:
-                stft = stft[:, :2]
-            sess = self._get_session()
-            outputs = sess.run(
-                outputs,
-                feed_dict=self._get_input_provider().get_feed_dict(
-                    features, stft, audio_descriptor
-                ),
-            )
-            for inst in self._get_builder().instruments:
-                out[inst] = self._stft(
-                    outputs[inst], inverse=True, length=waveform.shape[0]
-                )
-            return out
-
     def _separate_tensorflow(
         self, waveform: np.ndarray, audio_descriptor: AudioDescriptor
     ) -> Dict:
         """
         Performs source separation over the given waveform with tensorflow
         backend.
 
         Parameters:
-            waveform (numpy.ndarray):
+            waveform (np.ndarray):
                 Waveform to be separated (as a numpy array)
             audio_descriptor (AudioDescriptor):
+                Audio descriptor to be used.
 
         Returns:
-            Separated waveforms.
+            Dict:
+                Separated waveforms.
         """
         if not waveform.shape[-1] == 2:
             waveform = to_stereo(waveform)
         prediction_generator = self._get_prediction_generator()
         # NOTE: update data in generator before performing separation.
         self._data_generator.update_data(
             {"waveform": waveform, "audio_id": np.array(audio_descriptor)}
@@ -300,37 +220,36 @@
         # NOTE: perform separation.
         prediction = next(prediction_generator)
         prediction.pop("audio_id")
         return prediction
 
     def separate(
         self, waveform: np.ndarray, audio_descriptor: Optional[str] = ""
-    ) -> None:
+    ) -> Dict:
         """
         Performs separation on a waveform.
 
         Parameters:
-            waveform (numpy.ndarray):
+            waveform (np.ndarray):
                 Waveform to be separated (as a numpy array)
-            audio_descriptor (str):
+            audio_descriptor (Optional[str]):
                 (Optional) string describing the waveform (e.g. filename).
+
+        Returns:
+            Dict:
+                Separated waveforms.
         """
-        backend: str = self._params["stft_backend"]
-        if backend == STFTBackend.TENSORFLOW:
-            return self._separate_tensorflow(waveform, audio_descriptor)
-        elif backend == STFTBackend.LIBROSA:
-            return self._separate_librosa(waveform, audio_descriptor)
-        raise ValueError(f"Unsupported STFT backend {backend}")
+        return self._separate_tensorflow(waveform, audio_descriptor)
 
     def separate_to_file(
         self,
         audio_descriptor: AudioDescriptor,
         destination: str,
         audio_adapter: Optional[AudioAdapter] = None,
-        offset: int = 0,
+        offset: float = 0,
         duration: float = 600.0,
         codec: Codec = Codec.WAV,
         bitrate: str = "128k",
         filename_format: str = "{filename}/{instrument}.{codec}",
         synchronous: bool = True,
     ) -> None:
         """
@@ -348,15 +267,15 @@
         Parameters:
             audio_descriptor (AudioDescriptor):
                 Describe song to separate, used by audio adapter to
                 retrieve and load audio data, in case of file based
                 audio adapter, such descriptor would be a file path.
             destination (str):
                 Target directory to write output to.
-            audio_adapter (Optional[AudioAdapter]):
+            audio_adapter (AudioAdapter):
                 (Optional) Audio adapter to use for I/O.
             offset (int):
                 (Optional) Offset of loaded song.
             duration (float):
                 (Optional) Duration of loaded song (default: 600s).
             codec (Codec):
                 (Optional) Export codec.
```

### Comparing `spleeter-2.3.2/spleeter/utils/configuration.py` & `spleeter-2.4.0/spleeter/utils/configuration.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,37 +1,31 @@
 #!/usr/bin/env python
 # coding: utf8
 
 """ Module that provides configuration loading function. """
 
+import importlib.resources as loader
 import json
 from os.path import exists
 from typing import Dict
 
-try:
-    import importlib.resources as loader
-except ImportError:
-    # Try backported to PY<37 `importlib_resources`.
-    # pyright: reportMissingImports=false
-    import importlib_resources as loader
-
 from .. import SpleeterError, resources
 
 __email__ = "spleeter@deezer.com"
 __author__ = "Deezer Research"
 __license__ = "MIT License"
 
 _EMBEDDED_CONFIGURATION_PREFIX: str = "spleeter:"
 
 
 def load_configuration(descriptor: str) -> Dict:
     """
-    Load configuration from the given descriptor. Could be either a
-    `spleeter:` prefixed embedded configuration name or a file system path
-    to read configuration from.
+    Load configuration from the given descriptor.
+    Could be either a `spleeter:` prefixed embedded configuration name
+    or a file system path to read configuration from.
 
     Parameters:
         descriptor (str):
             Configuration descriptor to use for lookup.
 
     Returns:
         Dict:
```

### Comparing `spleeter-2.3.2/spleeter/utils/logging.py` & `spleeter-2.4.0/spleeter/utils/logging.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 # coding: utf8
 
-""" Centralized logging facilities for Spleeter. """
+"""Centralized logging facilities for Spleeter."""
 
 import logging
 import warnings
 from os import environ
 
 # pyright: reportMissingImports=false
 # pylint: disable=import-error
@@ -39,16 +39,16 @@
     """
     Configure application logger.
 
     Parameters:
         verbose (bool):
             `True` to use verbose logger, `False` otherwise.
     """
-    from tensorflow import get_logger
-    from tensorflow.compat.v1 import logging as tf_logging
+    from tensorflow import get_logger  # type: ignore
+    from tensorflow.compat.v1 import logging as tf_logging  # type: ignore
 
     tf_logger = get_logger()
     tf_logger.handlers = [handler]
     if verbose:
         tf_logging.set_verbosity(tf_logging.INFO)
         logger.setLevel(logging.DEBUG)
     else:
```

### Comparing `spleeter-2.3.2/spleeter/utils/tensor.py` & `spleeter-2.4.0/spleeter/utils/tensor.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,53 +1,53 @@
 #!/usr/bin/env python
 # coding: utf8
 
 """ Utility function for tensorflow. """
 
 from typing import Any, Callable, Dict
 
-import pandas as pd
+import pandas as pd  # type: ignore
 
 # pyright: reportMissingImports=false
 # pylint: disable=import-error
-import tensorflow as tf
+import tensorflow as tf  # type: ignore
 
 # pylint: enable=import-error
 
 __email__ = "spleeter@deezer.com"
 __author__ = "Deezer Research"
 __license__ = "MIT License"
 
 
 def sync_apply(
-    tensor_dict: tf.Tensor, func: Callable, concat_axis: int = 1
+    tensor_dict: Dict[str, tf.Tensor], func: Callable, concat_axis: int = 1
 ) -> Dict[str, tf.Tensor]:
     """
     Return a function that applies synchronously the provided func on the
     provided dictionnary of tensor. This means that func is applied to the
     concatenation of the tensors in tensor_dict. This is useful for
     performing random operation that needs the same drawn value on multiple
     tensor, such as a random time-crop on both input data and label (the
     same crop should be applied to both input data and label, so random
     crop cannot be applied separately on each of them).
 
-    Notes:
+    Note:
         All tensor are assumed to be the same shape.
 
     Parameters:
-        tensor_dict (Dict[str, tensorflow.Tensor]):
+        tensor_dict (Dict[str, tf.Tensor]):
             A dictionary of tensor.
         func (Callable):
             Function to be applied to the concatenation of the tensors in
             `tensor_dict`.
         concat_axis (int):
-            The axis on which to perform the concatenation.
+            (Optional) The axis on which to perform the concatenation.
 
     Returns:
-        Dict[str, tensorflow.Tensor]:
+        Dict[str, tf.Tensor]:
             Processed tensors dictionary with the same name (keys) as input
             tensor_dict.
     """
     if concat_axis not in {0, 1}:
         raise NotImplementedError(
             "Function only implemented for concat_axis equal to 0 or 1"
         )
@@ -69,25 +69,14 @@
 
 def from_float32_to_uint8(
     tensor: tf.Tensor,
     tensor_key: str = "tensor",
     min_key: str = "min",
     max_key: str = "max",
 ) -> tf.Tensor:
-    """
-
-    Parameters:
-        tensor (tensorflow.Tensor):
-        tensor_key (str):
-        min_key (str):
-        max_key (str):
-
-    Returns:
-        tensorflow.Tensor:
-    """
     tensor_min = tf.reduce_min(tensor)
     tensor_max = tf.reduce_max(tensor)
     return {
         tensor_key: tf.cast(
             (tensor - tensor_min) / (tensor_max - tensor_min + 1e-16) * 255.9999,
             dtype=tf.uint8,
         ),
@@ -95,87 +84,68 @@
         max_key: tensor_max,
     }
 
 
 def from_uint8_to_float32(
     tensor: tf.Tensor, tensor_min: tf.Tensor, tensor_max: tf.Tensor
 ) -> tf.Tensor:
-    """
-
-    Parameters:
-        tensor (tensorflow.Tensor):
-        tensor_min (tensorflow.Tensor):
-        tensor_max (tensorflow.Tensor):
-
-    Returns:
-        tensorflow.Tensor:
-    """
     return (
         tf.cast(tensor, tf.float32) * (tensor_max - tensor_min) / 255.9999 + tensor_min
     )
 
 
 def pad_and_partition(tensor: tf.Tensor, segment_len: int) -> tf.Tensor:
     """
     Pad and partition a tensor into segment of len `segment_len`
     along the first dimension. The tensor is padded with 0 in order
     to ensure that the first dimension is a multiple of `segment_len`.
 
-    Tensor must be of known fixed rank
-
     Examples:
-
-        ```python
-        >>> tensor = [[1, 2, 3], [4, 5, 6]]
-        >>> segment_len = 2
-        >>> pad_and_partition(tensor, segment_len)
-        [[[1, 2], [4, 5]], [[3, 0], [6, 0]]]
-        ````
+    ```python
+    >>> tensor = [[1, 2, 3], [4, 5, 6]]
+    >>> segment_len = 2
+    >>> pad_and_partition(tensor, segment_len)
+    [[[1, 2], [4, 5]], [[3, 0], [6, 0]]]
+    ````
 
     Parameters:
-        tensor (tensorflow.Tensor):
+        tensor (tf.Tensor):
+            Tensor of known fixed rank
         segment_len (int):
+            Segment length.
 
     Returns:
-        tensorflow.Tensor:
+        tf.Tensor:
+            Padded and partitioned tensor.
     """
     tensor_size = tf.math.floormod(tf.shape(tensor)[0], segment_len)
     pad_size = tf.math.floormod(segment_len - tensor_size, segment_len)
     padded = tf.pad(tensor, [[0, pad_size]] + [[0, 0]] * (len(tensor.shape) - 1))
     split = (tf.shape(padded)[0] + segment_len - 1) // segment_len
     return tf.reshape(
         padded, tf.concat([[split, segment_len], tf.shape(padded)[1:]], axis=0)
     )
 
 
 def pad_and_reshape(instr_spec, frame_length, F) -> Any:
-    """
-    Parameters:
-        instr_spec:
-        frame_length:
-        F:
-
-    Returns:
-        Any:
-    """
     spec_shape = tf.shape(instr_spec)
     extension_row = tf.zeros((spec_shape[0], spec_shape[1], 1, spec_shape[-1]))
     n_extra_row = (frame_length) // 2 + 1 - F
     extension = tf.tile(extension_row, [1, 1, n_extra_row, 1])
     extended_spec = tf.concat([instr_spec, extension], axis=2)
     old_shape = tf.shape(extended_spec)
     new_shape = tf.concat([[old_shape[0] * old_shape[1]], old_shape[2:]], axis=0)
     processed_instr_spec = tf.reshape(extended_spec, new_shape)
     return processed_instr_spec
 
 
 def dataset_from_csv(csv_path: str, **kwargs) -> Any:
     """
-    Load dataset from a CSV file using Pandas. kwargs if any are
-    forwarded to the `pandas.read_csv` function.
+    Load dataset from a CSV file using Pandas.
+    kwargs if any are forwarded to the `pandas.read_csv` function.
 
     Parameters:
         csv_path (str):
             Path of the CSV file to load dataset from.
 
     Returns:
         Any:
@@ -185,16 +155,16 @@
     dataset = tf.data.Dataset.from_tensor_slices({key: df[key].values for key in df})
     return dataset
 
 
 def check_tensor_shape(tensor_tf: tf.Tensor, target_shape: Any) -> bool:
     """
     Return a Tensorflow boolean graph that indicates whether
-    sample[features_key] has the specified target shape. Only check
-    not None entries of target_shape.
+    sample[features_key] has the specified target shape.
+    Only check not None entries of target_shape.
 
     Parameters:
         tensor_tf (tensorflow.Tensor):
             Tensor to check shape for.
         target_shape (Any):
             Target shape to compare tensor to.
 
@@ -209,22 +179,21 @@
                 result, tf.equal(tf.constant(target_length), tf.shape(tensor_tf)[i])
             )
     return result
 
 
 def set_tensor_shape(tensor: tf.Tensor, tensor_shape: Any) -> tf.Tensor:
     """
-    Set shape for a tensor (not in place, as opposed to tf.set_shape)
+    Set shape for a tensor (not in place, as opposed to tf.set_shape).
 
     Parameters:
         tensor (tensorflow.Tensor):
             Tensor to reshape.
         tensor_shape (Any):
             Shape to apply to the tensor.
 
     Returns:
         tensorflow.Tensor:
             A reshaped tensor.
     """
-    # NOTE: That SOUND LIKE IN PLACE HERE ?
     tensor.set_shape(tensor_shape)
     return tensor
```

### Comparing `spleeter-2.3.2/setup.py` & `spleeter-2.4.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,55 +1,187 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
-
-packages = \
-['spleeter',
- 'spleeter.audio',
- 'spleeter.model',
- 'spleeter.model.functions',
- 'spleeter.model.provider',
- 'spleeter.resources',
- 'spleeter.utils']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['ffmpeg-python==0.2.0',
- 'httpx[http2]>=0.19.0,<0.20.0',
- 'librosa>=0.8.0,<0.9.0',
- 'llvmlite>=0.38.0,<0.39.0',
- 'norbert==0.2.1',
- 'numpy>=1.19.2,<2.0.0',
- 'pandas>=1.2,<2.0',
- 'protobuf>=3.19.4,<4.0.0',
- 'tensorflow>=2.5.0,<3.0.0',
- 'typer>=0.3.2,<0.4.0']
-
-extras_require = \
-{':python_version < "3.7"': ['importlib-resources>=4.1.1,<5.0.0'],
- ':python_version < "3.8"': ['importlib-metadata>=3.0.0,<4.0.0'],
- 'evaluation': ['musdb==0.3.1', 'museval==0.3.0']}
-
-entry_points = \
-{'console_scripts': ['spleeter = spleeter.__main__:entrypoint']}
-
-setup_kwargs = {
-    'name': 'spleeter',
-    'version': '2.3.2',
-    'description': 'The Deezer source separation library with pretrained models based on tensorflow.',
-    'long_description': '<img src="https://github.com/deezer/spleeter/raw/master/images/spleeter_logo.png" height="80" />\n\n[![Github actions](https://github.com/deezer/spleeter/workflows/pytest/badge.svg)](https://github.com/deezer/spleeter/actions) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/spleeter) [![PyPI version](https://badge.fury.io/py/spleeter.svg)](https://badge.fury.io/py/spleeter) [![Conda](https://img.shields.io/conda/vn/deezer-research/spleeter)](https://anaconda.org/deezer-research/spleeter) [![Docker Pulls](https://img.shields.io/docker/pulls/deezer/spleeter)](https://hub.docker.com/r/deezer/spleeter) [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/deezer/spleeter/blob/master/spleeter.ipynb) [![Gitter chat](https://badges.gitter.im/gitterHQ/gitter.png)](https://gitter.im/spleeter/community) [![status](https://joss.theoj.org/papers/259e5efe669945a343bad6eccb89018b/status.svg)](https://joss.theoj.org/papers/259e5efe669945a343bad6eccb89018b)\n\n> :warning: [Spleeter 2.1.0](https://pypi.org/project/spleeter/) release introduces some breaking changes, including new CLI option naming for input, and the drop\n> of dedicated GPU package. Please read [CHANGELOG](CHANGELOG.md) for more details.\n\n## About\n\n**Spleeter** is [Deezer](https://www.deezer.com/) source separation library with pretrained models\nwritten in [Python](https://www.python.org/) and uses [Tensorflow](https://tensorflow.org/). It makes it easy\nto train source separation model (assuming you have a dataset of isolated sources), and provides\nalready trained state of the art model for performing various flavour of separation :\n\n* Vocals (singing voice) / accompaniment separation ([2 stems](https://github.com/deezer/spleeter/wiki/2.-Getting-started#using-2stems-model))\n* Vocals / drums / bass / other separation ([4 stems](https://github.com/deezer/spleeter/wiki/2.-Getting-started#using-4stems-model))\n* Vocals / drums / bass / piano / other separation ([5 stems](https://github.com/deezer/spleeter/wiki/2.-Getting-started#using-5stems-model))\n\n2 stems and 4 stems models have [high performances](https://github.com/deezer/spleeter/wiki/Separation-Performances) on the [musdb](https://sigsep.github.io/datasets/musdb.html) dataset. **Spleeter** is also very fast as it can perform separation of audio files to 4 stems 100x faster than real-time when run on a GPU.\n\nWe designed **Spleeter** so you can use it straight from [command line](https://github.com/deezer/spleeter/wiki/2.-Getting-started#usage)\nas well as directly in your own development pipeline as a [Python library](https://github.com/deezer/spleeter/wiki/4.-API-Reference#separator). It can be installed with [pip](https://github.com/deezer/spleeter/wiki/1.-Installation#using-pip) or be used with\n[Docker](https://github.com/deezer/spleeter/wiki/2.-Getting-started#using-docker-image).\n\n### Projects and Softwares using **Spleeter**\n\nSince it\'s been released, there are multiple forks exposing **Spleeter** through either a Guided User Interface (GUI) or a standalone free or paying website. Please note that we do not host, maintain or directly support any of these initiatives.\n\nThat being said, many cool projects have been built on top of ours. Notably the porting to the *Ableton Live* ecosystem through the [Spleeter 4 Max](https://github.com/diracdeltas/spleeter4max#spleeter-for-max) project.\n\n**Spleeter** pre-trained models have also been used by professionnal audio softwares. Here\'s a non-exhaustive list:\n\n* [iZotope](https://www.izotope.com/en/shop/rx-8-standard.html) in its *Music Rebalance* feature within **RX 8**\n* [SpectralLayers](https://new.steinberg.net/spectralayers/) in its *Unmix* feature in **SpectralLayers 7**\n* [Acon Digital](https://acondigital.com/products/acoustica-audio-editor/) within **Acoustica 7**\n* [VirtualDJ](https://www.virtualdj.com/stems/) in their stem isolation feature\n* [Algoriddim](https://www.algoriddim.com/apps) in their **NeuralMix** and **djayPRO** app suite\n\n🆕 **Spleeter** is a baseline in the ongoing [Music Demixing Challenge](https://www.aicrowd.com/challenges/music-demixing-challenge-ismir-2021)!\n\n## Quick start\n\nWant to try it out but don\'t want to install anything ? We have set up a [Google Colab](https://colab.research.google.com/github/deezer/spleeter/blob/master/spleeter.ipynb).\n\nReady to dig into it ? In a few lines you can install **Spleeter**  and separate the vocal and accompaniment parts from an example audio file.\nYou need first to install `ffmpeg` and `libsndfile`. It can be done on most platform using [Conda](https://github.com/deezer/spleeter/wiki/1.-Installation#using-conda):\n\n```bash\n# install dependencies using conda\nconda install -c conda-forge ffmpeg libsndfile\n# install spleeter with pip\npip install spleeter\n# download an example audio file (if you don\'t have wget, use another tool for downloading)\nwget https://github.com/deezer/spleeter/raw/master/audio_example.mp3\n# separate the example audio into two components\nspleeter separate -p spleeter:2stems -o output audio_example.mp3\n```\n\n> :warning: Note that we no longer recommend using `conda` for installing spleeter.\n\n> ⚠️ There are known issues with Apple M1 chips, mostly due to TensorFlow compatibility. Until these are fixed, you can use [this workaround](https://github.com/deezer/spleeter/issues/607#issuecomment-1021669444).\n\nYou should get two separated audio files (`vocals.wav` and `accompaniment.wav`) in the `output/audio_example` folder.\n\nFor a detailed documentation, please check the [repository wiki](https://github.com/deezer/spleeter/wiki/1.-Installation)\n\n## Development and Testing\n\nThis project is managed using [Poetry](https://python-poetry.org/docs/basic-usage/), to run test suite you\ncan execute the following set of commands:\n\n```bash\n# Clone spleeter repository\ngit clone https://github.com/Deezer/spleeter && cd spleeter\n# Install poetry\npip install poetry\n# Install spleeter dependencies\npoetry install\n# Run unit test suite\npoetry run pytest tests/\n```\n\n## Reference\n\n* Deezer Research - Source Separation Engine Story - deezer.io blog post:\n  * [English version](https://deezer.io/releasing-spleeter-deezer-r-d-source-separation-engine-2b88985e797e)\n  * [Japanese version](http://dzr.fm/splitterjp)\n* [Music Source Separation tool with pre-trained models / ISMIR2019 extended abstract](http://archives.ismir.net/ismir2019/latebreaking/000036.pdf)\n\nIf you use **Spleeter** in your work, please cite:\n\n```BibTeX\n@article{spleeter2020,\n  doi = {10.21105/joss.02154},\n  url = {https://doi.org/10.21105/joss.02154},\n  year = {2020},\n  publisher = {The Open Journal},\n  volume = {5},\n  number = {50},\n  pages = {2154},\n  author = {Romain Hennequin and Anis Khlif and Felix Voituret and Manuel Moussallam},\n  title = {Spleeter: a fast and efficient music source separation tool with pre-trained models},\n  journal = {Journal of Open Source Software},\n  note = {Deezer Research}\n}\n```\n\n## License\n\nThe code of **Spleeter** is [MIT-licensed](LICENSE).\n\n## Disclaimer\n\nIf you plan to use **Spleeter** on copyrighted material, make sure you get proper authorization from right owners beforehand.\n\n## Troubleshooting\n\n**Spleeter** is a complex piece of software and although we continously try to improve and test it you may encounter unexpected issues running it. If that\'s the case please check the [FAQ page](https://github.com/deezer/spleeter/wiki/5.-FAQ) first as well as the list of [currently open issues](https://github.com/deezer/spleeter/issues)\n\n### Windows users\n\n   It appears that sometimes the shortcut command `spleeter` does not work properly on windows. This is a known issue that we will hopefully fix soon. In the meantime replace `spleeter separate` by `python -m spleeter separate` in command line and it should work.\n\n## Contributing\n\nIf you would like to participate in the development of **Spleeter** you are more than welcome to do so. Don\'t hesitate to throw us a pull request and we\'ll do our best to examine it quickly. Please check out our [guidelines](.github/CONTRIBUTING.md) first.\n\n## Note\n\nThis repository include a demo audio file `audio_example.mp3` which is an excerpt\nfrom Slow Motion Dream by Steven M Bryant (c) copyright 2011 Licensed under a Creative\nCommons Attribution (3.0) [license](http://dig.ccmixter.org/files/stevieb357/34740)\nFt: CSoul,Alex Beroza & Robert Siekawitch\n',
-    'author': 'Deezer Research',
-    'author_email': 'spleeter@deezer.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/deezer/spleeter',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'extras_require': extras_require,
-    'entry_points': entry_points,
-    'python_requires': '>=3.7.1,<3.11',
+Metadata-Version: 2.1
+Name: spleeter
+Version: 2.4.0
+Summary: The Deezer source separation library with pretrained models based on tensorflow.
+Home-page: https://github.com/deezer/spleeter
+License: MIT
+Author: Deezer Research
+Author-email: spleeter@deezer.com
+Requires-Python: >=3.7.1,<3.11
+Classifier: Environment :: Console
+Classifier: Environment :: MacOS X
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Information Technology
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Operating System :: MacOS
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Operating System :: Unix
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Topic :: Artistic Software
+Classifier: Topic :: Multimedia
+Classifier: Topic :: Multimedia :: Sound/Audio
+Classifier: Topic :: Multimedia :: Sound/Audio :: Analysis
+Classifier: Topic :: Multimedia :: Sound/Audio :: Conversion
+Classifier: Topic :: Multimedia :: Sound/Audio :: Sound Synthesis
+Classifier: Topic :: Scientific/Engineering
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Classifier: Topic :: Scientific/Engineering :: Information Analysis
+Classifier: Topic :: Software Development
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: Utilities
+Provides-Extra: evaluation
+Requires-Dist: ffmpeg-python (>=0.2.0,<0.3.0)
+Requires-Dist: httpx[http2] (>=0.19.0,<0.20.0)
+Requires-Dist: musdb (>=0.4.0,<0.5.0) ; extra == "evaluation"
+Requires-Dist: museval (>=0.4.0,<0.5.0) ; extra == "evaluation"
+Requires-Dist: norbert (>=0.2.1,<0.3.0)
+Requires-Dist: pandas (>=1.3.0,<2.0.0)
+Requires-Dist: tensorflow (>=2.5.0,<2.10.0)
+Requires-Dist: typer (>=0.3.2,<0.4.0)
+Project-URL: Repository, https://github.com/deezer/spleeter
+Description-Content-Type: text/markdown
+
+<img src="https://github.com/deezer/spleeter/raw/master/images/spleeter_logo.png" height="80" />
+
+[![Github actions](https://github.com/deezer/spleeter/workflows/pytest/badge.svg)](https://github.com/deezer/spleeter/actions) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/spleeter) [![PyPI version](https://badge.fury.io/py/spleeter.svg)](https://badge.fury.io/py/spleeter) [![Conda](https://img.shields.io/conda/vn/deezer-research/spleeter)](https://anaconda.org/deezer-research/spleeter) [![Docker Pulls](https://img.shields.io/docker/pulls/deezer/spleeter)](https://hub.docker.com/r/deezer/spleeter) [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/deezer/spleeter/blob/master/spleeter.ipynb) [![Gitter chat](https://badges.gitter.im/gitterHQ/gitter.png)](https://gitter.im/spleeter/community) [![status](https://joss.theoj.org/papers/259e5efe669945a343bad6eccb89018b/status.svg)](https://joss.theoj.org/papers/259e5efe669945a343bad6eccb89018b)
+
+> :warning: [Spleeter 2.1.0](https://pypi.org/project/spleeter/) release introduces some breaking changes, including new CLI option naming for input, and the drop
+> of dedicated GPU package. Please read [CHANGELOG](CHANGELOG.md) for more details.
+
+## About
+
+**Spleeter** is [Deezer](https://www.deezer.com/) source separation library with pretrained models
+written in [Python](https://www.python.org/) and uses [Tensorflow](https://tensorflow.org/). It makes it easy
+to train source separation model (assuming you have a dataset of isolated sources), and provides
+already trained state of the art model for performing various flavour of separation :
+
+* Vocals (singing voice) / accompaniment separation ([2 stems](https://github.com/deezer/spleeter/wiki/2.-Getting-started#using-2stems-model))
+* Vocals / drums / bass / other separation ([4 stems](https://github.com/deezer/spleeter/wiki/2.-Getting-started#using-4stems-model))
+* Vocals / drums / bass / piano / other separation ([5 stems](https://github.com/deezer/spleeter/wiki/2.-Getting-started#using-5stems-model))
+
+2 stems and 4 stems models have [high performances](https://github.com/deezer/spleeter/wiki/Separation-Performances) on the [musdb](https://sigsep.github.io/datasets/musdb.html) dataset. **Spleeter** is also very fast as it can perform separation of audio files to 4 stems 100x faster than real-time when run on a GPU.
+
+We designed **Spleeter** so you can use it straight from [command line](https://github.com/deezer/spleeter/wiki/2.-Getting-started#usage)
+as well as directly in your own development pipeline as a [Python library](https://github.com/deezer/spleeter/wiki/4.-API-Reference#separator). It can be installed with [pip](https://github.com/deezer/spleeter/wiki/1.-Installation#using-pip) or be used with
+[Docker](https://github.com/deezer/spleeter/wiki/2.-Getting-started#using-docker-image).
+
+### Projects and Softwares using **Spleeter**
+
+Since it's been released, there are multiple forks exposing **Spleeter** through either a Guided User Interface (GUI) or a standalone free or paying website. Please note that we do not host, maintain or directly support any of these initiatives.
+
+That being said, many cool projects have been built on top of ours. Notably the porting to the *Ableton Live* ecosystem through the [Spleeter 4 Max](https://github.com/diracdeltas/spleeter4max#spleeter-for-max) project.
+
+**Spleeter** pre-trained models have also been used by professionnal audio softwares. Here's a non-exhaustive list:
+
+* [iZotope](https://www.izotope.com/en/shop/rx-8-standard.html) in its *Music Rebalance* feature within **RX 8**
+* [SpectralLayers](https://new.steinberg.net/spectralayers/) in its *Unmix* feature in **SpectralLayers 7**
+* [Acon Digital](https://acondigital.com/products/acoustica-audio-editor/) within **Acoustica 7**
+* [VirtualDJ](https://www.virtualdj.com/stems/) in their stem isolation feature
+* [Algoriddim](https://www.algoriddim.com/apps) in their **NeuralMix** and **djayPRO** app suite
+
+🆕 **Spleeter** is a baseline in the ongoing [Music Demixing Challenge](https://www.aicrowd.com/challenges/music-demixing-challenge-ismir-2021)!
+
+## Quick start
+
+Want to try it out but don't want to install anything ? We have set up a [Google Colab](https://colab.research.google.com/github/deezer/spleeter/blob/master/spleeter.ipynb).
+
+Ready to dig into it ? In a few lines you can install **Spleeter**  and separate the vocal and accompaniment parts from an example audio file.
+You need first to install `ffmpeg` and `libsndfile`. It can be done on most platform using [Conda](https://github.com/deezer/spleeter/wiki/1.-Installation#using-conda):
+
+```bash
+# install dependencies using conda
+conda install -c conda-forge ffmpeg libsndfile
+# install spleeter with pip
+pip install spleeter
+# download an example audio file (if you don't have wget, use another tool for downloading)
+wget https://github.com/deezer/spleeter/raw/master/audio_example.mp3
+# separate the example audio into two components
+spleeter separate -p spleeter:2stems -o output audio_example.mp3
+```
+
+> :warning: Note that we no longer recommend using `conda` for installing spleeter.
+
+> ⚠️ There are known issues with Apple M1 chips, mostly due to TensorFlow compatibility. Until these are fixed, you can use [this workaround](https://github.com/deezer/spleeter/issues/607#issuecomment-1021669444).
+
+You should get two separated audio files (`vocals.wav` and `accompaniment.wav`) in the `output/audio_example` folder.
+
+For a detailed documentation, please check the [repository wiki](https://github.com/deezer/spleeter/wiki/1.-Installation)
+
+## Development and Testing
+
+This project is managed using [Poetry](https://python-poetry.org/docs/basic-usage/), to run test suite you
+can execute the following set of commands:
+
+```bash
+# Clone spleeter repository
+git clone https://github.com/Deezer/spleeter && cd spleeter
+# Install poetry
+pip install poetry
+# Install spleeter dependencies
+poetry install
+# Run unit test suite
+poetry run pytest tests/
+```
+
+## Reference
+
+* Deezer Research - Source Separation Engine Story - deezer.io blog post:
+  * [English version](https://deezer.io/releasing-spleeter-deezer-r-d-source-separation-engine-2b88985e797e)
+  * [Japanese version](http://dzr.fm/splitterjp)
+* [Music Source Separation tool with pre-trained models / ISMIR2019 extended abstract](http://archives.ismir.net/ismir2019/latebreaking/000036.pdf)
+
+If you use **Spleeter** in your work, please cite:
+
+```BibTeX
+@article{spleeter2020,
+  doi = {10.21105/joss.02154},
+  url = {https://doi.org/10.21105/joss.02154},
+  year = {2020},
+  publisher = {The Open Journal},
+  volume = {5},
+  number = {50},
+  pages = {2154},
+  author = {Romain Hennequin and Anis Khlif and Felix Voituret and Manuel Moussallam},
+  title = {Spleeter: a fast and efficient music source separation tool with pre-trained models},
+  journal = {Journal of Open Source Software},
+  note = {Deezer Research}
 }
+```
+
+## License
+
+The code of **Spleeter** is [MIT-licensed](LICENSE).
+
+## Disclaimer
+
+If you plan to use **Spleeter** on copyrighted material, make sure you get proper authorization from right owners beforehand.
+
+## Troubleshooting
+
+**Spleeter** is a complex piece of software and although we continously try to improve and test it you may encounter unexpected issues running it. If that's the case please check the [FAQ page](https://github.com/deezer/spleeter/wiki/5.-FAQ) first as well as the list of [currently open issues](https://github.com/deezer/spleeter/issues)
+
+### Windows users
+
+   It appears that sometimes the shortcut command `spleeter` does not work properly on windows. This is a known issue that we will hopefully fix soon. In the meantime replace `spleeter separate` by `python -m spleeter separate` in command line and it should work.
+
+## Contributing
+
+If you would like to participate in the development of **Spleeter** you are more than welcome to do so. Don't hesitate to throw us a pull request and we'll do our best to examine it quickly. Please check out our [guidelines](.github/CONTRIBUTING.md) first.
+
+## Note
 
+This repository include a demo audio file `audio_example.mp3` which is an excerpt
+from Slow Motion Dream by Steven M Bryant (c) copyright 2011 Licensed under a Creative
+Commons Attribution (3.0) [license](http://dig.ccmixter.org/files/stevieb357/34740)
+Ft: CSoul,Alex Beroza & Robert Siekawitch
 
-setup(**setup_kwargs)
```

