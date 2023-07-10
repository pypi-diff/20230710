# Comparing `tmp/synthax-0.1.2.tar.gz` & `tmp/synthax-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "synthax-0.1.2.tar", last modified: Thu Jun 22 23:10:22 2023, max compression
+gzip compressed data, was "synthax-0.2.0.tar", last modified: Mon Jul 10 18:49:17 2023, max compression
```

## Comparing `synthax-0.1.2.tar` & `synthax-0.2.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 23:10:22.553551 synthax-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-22 23:10:13.000000 synthax-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3120 2023-06-22 23:10:22.553551 synthax-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-06-22 23:10:13.000000 synthax-0.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 23:10:22.553551 synthax-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-06-22 23:10:13.000000 synthax-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 23:10:22.545551 synthax-0.1.2/synthax/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 23:10:13.000000 synthax-0.1.2/synthax/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2678 2023-06-22 23:10:13.000000 synthax-0.1.2/synthax/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-06-22 23:10:13.000000 synthax-0.1.2/synthax/functional.py
--rw-r--r--   0 runner    (1001) docker     (123)     4076 2023-06-22 23:10:13.000000 synthax-0.1.2/synthax/io.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 23:10:22.553551 synthax-0.1.2/synthax/modules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 23:10:13.000000 synthax-0.1.2/synthax/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-06-22 23:10:13.000000 synthax-0.1.2/synthax/modules/amplifiers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5758 2023-06-22 23:10:13.000000 synthax-0.1.2/synthax/modules/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4745 2023-06-22 23:10:13.000000 synthax-0.1.2/synthax/modules/blend.py
--rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-06-22 23:10:13.000000 synthax-0.1.2/synthax/modules/control.py
--rw-r--r--   0 runner    (1001) docker     (123)     7299 2023-06-22 23:10:13.000000 synthax-0.1.2/synthax/modules/envelopes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-06-22 23:10:13.000000 synthax-0.1.2/synthax/modules/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-06-22 23:10:13.000000 synthax-0.1.2/synthax/modules/keyboard.py
--rw-r--r--   0 runner    (1001) docker     (123)     6297 2023-06-22 23:10:13.000000 synthax-0.1.2/synthax/modules/lfos.py
--rw-r--r--   0 runner    (1001) docker     (123)     5495 2023-06-22 23:10:13.000000 synthax-0.1.2/synthax/modules/mixers.py
--rw-r--r--   0 runner    (1001) docker     (123)    12272 2023-06-22 23:10:13.000000 synthax-0.1.2/synthax/modules/oscillators.py
--rw-r--r--   0 runner    (1001) docker     (123)     4871 2023-06-22 23:10:13.000000 synthax-0.1.2/synthax/parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)    19034 2023-06-22 23:10:13.000000 synthax-0.1.2/synthax/synth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-06-22 23:10:13.000000 synthax-0.1.2/synthax/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 23:10:22.549551 synthax-0.1.2/synthax.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3120 2023-06-22 23:10:22.000000 synthax-0.1.2/synthax.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-06-22 23:10:22.000000 synthax-0.1.2/synthax.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 23:10:22.000000 synthax-0.1.2/synthax.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-22 23:10:22.000000 synthax-0.1.2/synthax.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-22 23:10:22.000000 synthax-0.1.2/synthax.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:49:17.572657 synthax-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-10 18:49:08.000000 synthax-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-07-10 18:49:17.572657 synthax-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-07-10 18:49:08.000000 synthax-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 18:49:17.572657 synthax-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-07-10 18:49:08.000000 synthax-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:49:17.568657 synthax-0.2.0/synthax/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 18:49:08.000000 synthax-0.2.0/synthax/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2678 2023-07-10 18:49:08.000000 synthax-0.2.0/synthax/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-07-10 18:49:08.000000 synthax-0.2.0/synthax/functional.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4149 2023-07-10 18:49:08.000000 synthax-0.2.0/synthax/io.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:49:17.572657 synthax-0.2.0/synthax/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 18:49:08.000000 synthax-0.2.0/synthax/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-07-10 18:49:08.000000 synthax-0.2.0/synthax/modules/amplifiers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6429 2023-07-10 18:49:08.000000 synthax-0.2.0/synthax/modules/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4486 2023-07-10 18:49:08.000000 synthax-0.2.0/synthax/modules/blend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-07-10 18:49:08.000000 synthax-0.2.0/synthax/modules/control.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7588 2023-07-10 18:49:08.000000 synthax-0.2.0/synthax/modules/envelopes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-07-10 18:49:08.000000 synthax-0.2.0/synthax/modules/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-07-10 18:49:08.000000 synthax-0.2.0/synthax/modules/keyboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6687 2023-07-10 18:49:08.000000 synthax-0.2.0/synthax/modules/lfos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4710 2023-07-10 18:49:08.000000 synthax-0.2.0/synthax/modules/mixers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12041 2023-07-10 18:49:08.000000 synthax-0.2.0/synthax/modules/oscillators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5200 2023-07-10 18:49:08.000000 synthax-0.2.0/synthax/parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17520 2023-07-10 18:49:08.000000 synthax-0.2.0/synthax/synth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-07-10 18:49:08.000000 synthax-0.2.0/synthax/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:49:17.568657 synthax-0.2.0/synthax.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-07-10 18:49:17.000000 synthax-0.2.0/synthax.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-07-10 18:49:17.000000 synthax-0.2.0/synthax.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 18:49:17.000000 synthax-0.2.0/synthax.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-10 18:49:17.000000 synthax-0.2.0/synthax.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-10 18:49:17.000000 synthax-0.2.0/synthax.egg-info/top_level.txt
```

### Comparing `synthax-0.1.2/LICENSE` & `synthax-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `synthax-0.1.2/PKG-INFO` & `synthax-0.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: synthax
-Version: 0.1.2
+Version: 0.2.0
 Summary: SynthAX: A Fast Modular Synthesizer in JAX
 Home-page: https://github.com/PapayaResearch/synthax
 Author: Manuel Cherep, Nikhil Singh
 Author-email: mcherep@mit.edu, nsingh1@mit.edu
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -28,35 +28,32 @@
 
 ```python
 import jax
 from synthax.config import SynthConfig
 from synthax.synth import ParametricSynth
 
 # Generate PRNG key
-key = jax.random.PRNGKey(42)
 config = SynthConfig(
     batch_size=16,
     sample_rate=44100,
     buffer_size_seconds=4.0
 )
 
-key, subkey = jax.random.split(key)
 # Instantiate synthesizer
 synth = ParametricSynth(
-    PRNG_key=subkey,
     config=config,
     sine=1,
     square_saw=1,
     fm_sine=1,
     fm_square_saw=0
 )
 
-key, subkey = jax.random.split(key)
 # Initialize and run
-params = synth.init(subkey)
+key = jax.random.PRNGKey(42)
+params = synth.init(key)
 audio = jax.jit(synth.apply)(params)
 ```
 
 ## Installation
 
 The latest `synthax` release can directly be installed from PyPI:
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: synthax Version: 0.1.2 Summary: SynthAX: A Fast
+Metadata-Version: 2.1 Name: synthax Version: 0.2.0 Summary: SynthAX: A Fast
 Modular Synthesizer in JAX Home-page: https://github.com/PapayaResearch/synthax
 Author: Manuel Cherep, Nikhil Singh Author-email: mcherep@mit.edu,
 nsingh1@mit.edu Classifier: Programming Language :: Python :: 3.9 Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
 Independent Requires-Python: >=3.9 Description-Content-Type: text/markdown
 License-File: LICENSE # SynthAX: A Fast Modular Synthesizer in JAX â¡ï¸ [!
 [Pyversions](https://img.shields.io/pypi/pyversions/synthax.svg?style=flat-
@@ -17,25 +17,23 @@
 audio over 60,000 times faster than realtime, and significantly faster than the
 state-of-the-art in accelerated sound synthesis. It leverages massive
 vectorization and high-throughput accelerators. You can get started here [!
 [Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://
 colab.research.google.com/github/PapayaResearch/synthax/blob/main/examples/
 walkthrough.ipynb) ## Basic `synthax` API Usage ```python import jax from
 synthax.config import SynthConfig from synthax.synth import ParametricSynth #
-Generate PRNG key key = jax.random.PRNGKey(42) config = SynthConfig
-( batch_size=16, sample_rate=44100, buffer_size_seconds=4.0 ) key, subkey =
-jax.random.split(key) # Instantiate synthesizer synth = ParametricSynth
-( PRNG_key=subkey, config=config, sine=1, square_saw=1, fm_sine=1,
-fm_square_saw=0 ) key, subkey = jax.random.split(key) # Initialize and run
-params = synth.init(subkey) audio = jax.jit(synth.apply)(params) ``` ##
-Installation The latest `synthax` release can directly be installed from PyPI:
-``` pip install synthax ``` If you want to get the most recent commit, please
-install directly from the repository: ``` pip install git+https://github.com/
-PapayaResearch/synthax.git@main ``` In order to use JAX on your accelerators,
-you can find more details in the [JAX documentation](https://github.com/google/
-jax#installation). ## Acknowledgements & Citing If you use `synthax` in your
-research, please cite the following: ``` @software{synthax2023, author =
-{Cherep, Manuel and Singh, Nikhil}, title = {SynthAX: A Fast Modular
-Synthesizer in JAX}, url = {https://github.com/PapayaResearch/synthax}, version
-= {0.1.0}, year = {2023}, } ``` This project is based on [torchsynth](https://
-github.com/torchsynth/torchsynth). We acknowledge financial support by
-Fulbright Spain.
+Generate PRNG key config = SynthConfig( batch_size=16, sample_rate=44100,
+buffer_size_seconds=4.0 ) # Instantiate synthesizer synth = ParametricSynth
+( config=config, sine=1, square_saw=1, fm_sine=1, fm_square_saw=0 ) #
+Initialize and run key = jax.random.PRNGKey(42) params = synth.init(key) audio
+= jax.jit(synth.apply)(params) ``` ## Installation The latest `synthax` release
+can directly be installed from PyPI: ``` pip install synthax ``` If you want to
+get the most recent commit, please install directly from the repository: ```
+pip install git+https://github.com/PapayaResearch/synthax.git@main ``` In order
+to use JAX on your accelerators, you can find more details in the [JAX
+documentation](https://github.com/google/jax#installation). ## Acknowledgements
+& Citing If you use `synthax` in your research, please cite the following: ```
+@software{synthax2023, author = {Cherep, Manuel and Singh, Nikhil}, title =
+{SynthAX: A Fast Modular Synthesizer in JAX}, url = {https://github.com/
+PapayaResearch/synthax}, version = {0.1.0}, year = {2023}, } ``` This project
+is based on [torchsynth](https://github.com/torchsynth/torchsynth). We
+acknowledge financial support by Fulbright Spain.
```

### Comparing `synthax-0.1.2/README.md` & `synthax-0.2.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -14,35 +14,32 @@
 
 ```python
 import jax
 from synthax.config import SynthConfig
 from synthax.synth import ParametricSynth
 
 # Generate PRNG key
-key = jax.random.PRNGKey(42)
 config = SynthConfig(
     batch_size=16,
     sample_rate=44100,
     buffer_size_seconds=4.0
 )
 
-key, subkey = jax.random.split(key)
 # Instantiate synthesizer
 synth = ParametricSynth(
-    PRNG_key=subkey,
     config=config,
     sine=1,
     square_saw=1,
     fm_sine=1,
     fm_square_saw=0
 )
 
-key, subkey = jax.random.split(key)
 # Initialize and run
-params = synth.init(subkey)
+key = jax.random.PRNGKey(42)
+params = synth.init(key)
 audio = jax.jit(synth.apply)(params)
 ```
 
 ## Installation
 
 The latest `synthax` release can directly be installed from PyPI:
```

#### html2text {}

```diff
@@ -11,25 +11,23 @@
 audio over 60,000 times faster than realtime, and significantly faster than the
 state-of-the-art in accelerated sound synthesis. It leverages massive
 vectorization and high-throughput accelerators. You can get started here [!
 [Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://
 colab.research.google.com/github/PapayaResearch/synthax/blob/main/examples/
 walkthrough.ipynb) ## Basic `synthax` API Usage ```python import jax from
 synthax.config import SynthConfig from synthax.synth import ParametricSynth #
-Generate PRNG key key = jax.random.PRNGKey(42) config = SynthConfig
-( batch_size=16, sample_rate=44100, buffer_size_seconds=4.0 ) key, subkey =
-jax.random.split(key) # Instantiate synthesizer synth = ParametricSynth
-( PRNG_key=subkey, config=config, sine=1, square_saw=1, fm_sine=1,
-fm_square_saw=0 ) key, subkey = jax.random.split(key) # Initialize and run
-params = synth.init(subkey) audio = jax.jit(synth.apply)(params) ``` ##
-Installation The latest `synthax` release can directly be installed from PyPI:
-``` pip install synthax ``` If you want to get the most recent commit, please
-install directly from the repository: ``` pip install git+https://github.com/
-PapayaResearch/synthax.git@main ``` In order to use JAX on your accelerators,
-you can find more details in the [JAX documentation](https://github.com/google/
-jax#installation). ## Acknowledgements & Citing If you use `synthax` in your
-research, please cite the following: ``` @software{synthax2023, author =
-{Cherep, Manuel and Singh, Nikhil}, title = {SynthAX: A Fast Modular
-Synthesizer in JAX}, url = {https://github.com/PapayaResearch/synthax}, version
-= {0.1.0}, year = {2023}, } ``` This project is based on [torchsynth](https://
-github.com/torchsynth/torchsynth). We acknowledge financial support by
-Fulbright Spain.
+Generate PRNG key config = SynthConfig( batch_size=16, sample_rate=44100,
+buffer_size_seconds=4.0 ) # Instantiate synthesizer synth = ParametricSynth
+( config=config, sine=1, square_saw=1, fm_sine=1, fm_square_saw=0 ) #
+Initialize and run key = jax.random.PRNGKey(42) params = synth.init(key) audio
+= jax.jit(synth.apply)(params) ``` ## Installation The latest `synthax` release
+can directly be installed from PyPI: ``` pip install synthax ``` If you want to
+get the most recent commit, please install directly from the repository: ```
+pip install git+https://github.com/PapayaResearch/synthax.git@main ``` In order
+to use JAX on your accelerators, you can find more details in the [JAX
+documentation](https://github.com/google/jax#installation). ## Acknowledgements
+& Citing If you use `synthax` in your research, please cite the following: ```
+@software{synthax2023, author = {Cherep, Manuel and Singh, Nikhil}, title =
+{SynthAX: A Fast Modular Synthesizer in JAX}, url = {https://github.com/
+PapayaResearch/synthax}, version = {0.1.0}, year = {2023}, } ``` This project
+is based on [torchsynth](https://github.com/torchsynth/torchsynth). We
+acknowledge financial support by Fulbright Spain.
```

### Comparing `synthax-0.1.2/setup.py` & `synthax-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
 from setuptools import setup, find_packages
 
 setup(name="synthax",
-      version="0.1.2",
+      version="0.2.0",
       url="https://github.com/PapayaResearch/synthax",
       author="Manuel Cherep, Nikhil Singh",
       author_email="mcherep@mit.edu, nsingh1@mit.edu",
       description="SynthAX: A Fast Modular Synthesizer in JAX",
       long_description=open("README.md").read(),
       long_description_content_type="text/markdown",
       packages=find_packages(),
```

### Comparing `synthax-0.1.2/synthax/config.py` & `synthax-0.2.0/synthax/config.py`

 * *Files identical despite different names*

### Comparing `synthax-0.1.2/synthax/functional.py` & `synthax-0.2.0/synthax/functional.py`

 * *Files 23% similar despite different names*

```diff
@@ -17,59 +17,40 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 import jax
-import flax
 import jax.numpy as jnp
+import flax
 import chex
 from typing import Tuple
 from synthax.types import Signal
 
-
 def midi_to_hz(midi: chex.Array) -> chex.Array:
     """
     Convert from midi (linear pitch) to frequency in Hz.
 
     Args:
-        midi (TODO): Linear pitch on the MIDI scale.
+        midi (chex.Array): Linear pitch on the MIDI scale.
 
     Return:
         Frequency in Hz.
     """
     return 440.0 * (jnp.exp2((midi - 69.0) / 12.0))
 
 def normalize_if_clipping(signal: Signal) -> Signal:
     """
-    Only normalize invidiaul signals in batch that have samples
+    Only normalize individual signals in batch that have samples
     less than -1.0 or greater than 1.0
     """
     max_sample = jnp.max(jnp.abs(signal), axis=1, keepdims=True)[0]
     return jnp.where(max_sample > 1.0, signal / max_sample, signal)
 
 
 def normalize(signal: Signal) -> Signal:
     """
     Normalize every individual signal in batch.
     """
     max_sample = jnp.max(jnp.abs(signal), axis=1, keepdims=True)[0]
     return signal / max_sample
-
-def flatten_params(
-        params: flax.core.frozen_dict.FrozenDict
-) -> Tuple[dict, chex.Array]:
-    """
-    Takes flax params and returns flat keys and batch of values
-    """
-    flat_dict = flax.traverse_util.flatten_dict(params)
-    keys = flat_dict.keys()
-    values = jnp.array(list(flat_dict.values()))
-    return keys, values
-
-def unflatten_params(keys: dict, values: chex.Array) -> dict:
-    """
-    Reconstructs the params from keys and values. It can be
-    passed to functions expecting a FrozenDict, but it's not frozen.
-    """
-    return flax.traverse_util.unflatten_dict(dict(zip(keys, values)))
```

### Comparing `synthax-0.1.2/synthax/io.py` & `synthax-0.2.0/synthax/io.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,14 +36,15 @@
     PRNGkey: Optional[jax.random.PRNGKey]
 
 
 def write_synthspec(
     outfile: str,
     synth: BaseSynth,
     params: Optional[dict] = None,
+    PRNGkey: Optional[jax.random.PRNGKey] = None,
     format: str = "yaml",
     **kwargs
 ):
     """
     Write a synth spec to disk.
 
     Args:
@@ -68,15 +69,17 @@
     params = params_tovals(params)
 
     if params is not None:
         outd = {"params": params} if "params" not in params else dict(params)
 
     if synth is not None:
         outd["config"] = synth.config.__dict__
-        outd["prng_key"] = synth.PRNG_key.tolist()[-1]
+
+    if PRNGkey is not None:
+        outd["prng_key"] = PRNG_key.tolist()[-1]
 
     outdata = None
     if format in ("yaml", "yml"):
         outdata = yaml.dump(outd, Dumper=yaml.CDumper)
     elif format == "json":
         outdata = json.dumps(outd, indent=4)
     else:
```

### Comparing `synthax-0.1.2/synthax/modules/amplifiers.py` & `synthax-0.2.0/synthax/modules/amplifiers.py`

 * *Files 10% similar despite different names*

```diff
@@ -33,15 +33,14 @@
 
     The VCA shapes the amplitude of an audio input signal over time, as
     determined by a control signal. To shape control-rate signals, use
     :class:`synthax.module.ControlRateVCA`.
 
     Args:
         config (SynthConfig): See :class:`~synhtax.module.SynthModule`
-        PRNG_key (jax.random.PRNGKey): PRNG key already split.
     """
 
     def __call__(self, audio_in: Signal, control_in: Signal):
         signal = audio_in * control_in
         return signal
 
 
@@ -51,13 +50,12 @@
 
     The VCA shapes the amplitude of a control input signal over time, as
     determined by another control signal. To shape audio-rate signals, use
     :class:`synthax.module.VCA`.
 
     Args:
         config (SynthConfig): See :class:`~synhtax.module.SynthModule`
-        PRNG_key (jax.random.PRNGKey): PRNG key already split.
     """
 
     def __call__(self, audio_in: Signal, control_in: Signal):
         signal = audio_in * control_in
         return signal
```

### Comparing `synthax-0.1.2/synthax/modules/base.py` & `synthax-0.2.0/synthax/modules/base.py`

 * *Files 15% similar despite different names*

```diff
@@ -22,63 +22,84 @@
 
 import jax
 import jax.numpy as jnp
 import chex
 import dataclasses
 from flax import linen as nn
 from synthax.config import SynthConfig
-from synthax.parameter import ModuleParameter, ModuleParameterRange, ModuleParameterSpec, to_0to1
+from synthax.parameter import ModuleParameterRange, ModuleParameterSpec, to_0to1
 from synthax.types import Signal, is_parameter_spec
 
 
 class SynthModule(nn.Module):
     """
     A base class for synthesis modules. A :class:`~.SynthModule`
     optionally takes input from other :class:`~.SynthModule` instances.
-    The :class:`~.SynthModule` uses its (optional) input and its
-    set of :class:`~synthax.parameter.ModuleParameter` to generate
-    output.
 
     All :class:`~.SynthModule` objects should be atomic, i.e., they
     should not contain other :class:`~.SynthModule` objects. This
     design choice is in the spirit of modular synthesis.
 
     Args:
         config (SynthConfig): An object containing synthesis settings
             that are shared across all modules.
-        PRNG_key (jax.random.PRNGKey): PRNG key already split.
     """
 
     config: SynthConfig
-    PRNG_key: jax.random.PRNGKey
 
     def setup(self):
-        # Filter all ParameterSpec default values
-        default_values = {f.name: f.default
+        # Filter all ParameterSpec default ranges
+        default_ranges = {f.name: f.default
                           for f in dataclasses.fields(self) if is_parameter_spec(f.type)}
-        self.parameters = {
-            name: self._init_param(name, default_value)
-            for name, default_value in default_values.items()
-        }
-
-    def _init_param(self, param_name, default_rng):
-        param = getattr(self, param_name)
-        if isinstance(param, jnp.ndarray):
-            rng = default_rng
-            val = to_0to1(param, rng)
-        if isinstance(param, ModuleParameterRange):
-            rng = param
-            val = jax.random.uniform(
-                self.PRNG_key,
-                shape=(self.config.batch_size,)
+        for name, default_range in default_ranges.items():
+            self._init_param(name, default_range)
+
+    def _init_param(self, name, default_range, initializer=None):
+        def init_param(PRNG_key: jax.random.PRNGKey):
+            parameter_spec = getattr(self, name)
+            if isinstance(parameter_spec, jnp.ndarray):
+                # Values are assumed to be within the parameter range
+                parameter_range = default_range
+                value = parameter_spec
+            if isinstance(parameter_spec, ModuleParameterRange):
+                parameter_range = parameter_spec
+                if initializer is None:
+                    # Random initialization uniformly within the parameter range
+                    value = jax.random.uniform(
+                        PRNG_key,
+                        shape=(self.config.batch_size,),
+                        minval=parameter_range.minimum,
+                        maxval=parameter_range.maximum
+                    )
+                else:
+                    # Custom initialization
+                    value = initializer(PRNG_key, parameter_range)
+
+            if isinstance(parameter_spec, ModuleParameterSpec):
+                # Values are assumed to be within the parameter range
+                parameter_range = parameter_spec.range_
+                value = parameter_spec.value
+
+            setattr(
+                self,
+                "_"+name+"_range",
+                parameter_range
+            )
+
+            # Save value in 0-1 range
+            return to_0to1(value, parameter_range)
+
+        setattr(
+            self,
+            "_"+name,
+            self.param(
+                name,
+                lambda rng: init_param(rng)
             )
-        if isinstance(param, ModuleParameterSpec):
-            rng = param.range
-            val = to_0to1(param.value, rng)
-        return ModuleParameter(name=param_name, range=rng, value=val)
+        )
 
     @property
     def batch_size(self):
         """ Size of the batch to be generated. """
         return self.config.batch_size
 
     @property
@@ -118,15 +139,14 @@
     """
     An abstract base class for non-audio modules that adapts the functions of
     :class:`.~SynthModule` to run at :attr:`~.ControlRateModule.control_rate`.
 
     Args:
         config (SynthConfig): An object containing synthesis settings
             that are shared across all modules.
-        PRNG_key (jax.random.PRNGKey): PRNG key already split.
     """
 
     @property
     def sample_rate(self):
         raise NotImplementedError("This module operates at control rate")
 
     @property
```

### Comparing `synthax-0.1.2/synthax/modules/blend.py` & `synthax-0.2.0/synthax/modules/blend.py`

 * *Files 17% similar despite different names*

```diff
@@ -22,28 +22,27 @@
 
 import jax
 import jax.numpy as jnp
 import chex
 import dataclasses
 from flax import linen as nn
 from synthax.modules.base import SynthModule
-from synthax.parameter import ModuleParameter, ModuleParameterRange
+from synthax.parameter import ModuleParameterRange, from_0to1
 from synthax.config import SynthConfig
 from synthax.types import ParameterSpec
 from typing import Optional
 
 
 class CrossfadeKnob(SynthModule):
     """
     Crossfade knob parameter with no signal generation
 
     Args:
         config (:class:`~synthax.config.SynthConfig`): Configuration.
-        PRNG_key (jax.random.PRNGKey): PRNG key already split.
-        ratio (ParameterSpec): TODO
+        ratio (synthax.types.ParameterSpec): Accepts a parameter range, initial values or both.
     """
 
     ratio: Optional[ParameterSpec] = ModuleParameterRange(
         minimum=0.0,
         maximum=1.0,
     )
 
@@ -51,79 +50,75 @@
 class SoftModeSelector(SynthModule):
     """
     A soft mode selector.
     If there are n different modes, return a probability distribution over them.
 
     Args:
         config (:class:`~synthax.config.SynthConfig`): Global configuration.
-        PRNG_key (jax.random.PRNGKey): PRNG key already split.
-        n_modes (int): TODO
+        n_modes (int): Number of modes.
         exponent (chex.Array): determines how strongly to scale each [0,1] value prior to normalization.
-        parameter_ranges (:class:`~synthax.parameter.ModuleParameterRange`): TODO.
+        mode (synthax.types.ParameterSpec): Accepts a parameter range, initial values or both, for all modes equally.
     """
 
     n_modes: int
     exponent: chex.Array = jnp.exp(1), # e
     mode: Optional[ParameterSpec] = ModuleParameterRange(
         minimum=0.0,
         maximum=1.0,
     )
 
     def setup(self):
-        param_names = []
-        for i in range(self.n_modes):
-            param_name = f"mode{i}weight"
-            param_names.append(param_name)
-            setattr(self, param_name, self.mode)
         # The default parameter range applies to all modes
-        default_values = {f.name: f.default for f in dataclasses.fields(self)}
-        default_rng = default_values["mode"]
-        self.parameters = {
-            name: self._init_param(name, default_rng)
-            for name in param_names
-        }
+        default_ranges = {f.name: f.default for f in dataclasses.fields(self)}
+        default_range = default_ranges["mode"]
+        initializer = lambda PRNG_key, range_: jax.random.uniform(
+            PRNG_key,
+            shape=(self.n_modes, self.config.batch_size),
+            minval=range_.minimum,
+            maxval=range_.maximum
+        )
+        # Initialize the parameter
+        self._init_param("mode", default_range, initializer)
 
     def __call__(self):
         # Normalize all mode weights so they sum to 1.0
-        # TODO: Refactor get all values in SynthModule
-        parameter_values = [p.from_0to1() for k, p in self.parameters.items()]
-        parameter_values_exp = jnp.power(parameter_values, exponent=self.exponent)
-        return parameter_values_exp / jnp.sum(parameter_values_exp, axis=0)
+        values_exp = jnp.power(
+            from_0to1(self._mode, self._mode_range),
+            self.exponent[0]
+        )
+        return values_exp / jnp.sum(values_exp, axis=0)
 
 
 class HardModeSelector(SynthModule):
     """
     A hard mode selector.
     NOTE: This is non-differentiable.
 
     Args:
         config (SynthConfig): Global configuration.
-        PRNG_key (jax.random.PRNGKey): PRNG key already split.
-        n_modes (int): TODO
-        parameter_ranges (:class:`~synthax.parameter.ModuleParameterRange`): TODO.
+        n_modes (int): Number of modes.
+        mode (synthax.types.ParameterSpec): Accepts a parameter range, initial values or both, for all modes equally.
     """
 
     n_modes: int
     mode: Optional[ParameterSpec] = ModuleParameterRange(
         minimum=0.0,
         maximum=1.0,
     )
 
     def setup(self):
-        param_names = []
-        for i in range(self.n_modes):
-            param_name = f"mode{i}weight"
-            param_names.append(param_name)
-            setattr(self, param_name, self.mode)
         # The default parameter range applies to all modes
-        default_values = {f.name: f.default for f in dataclasses.fields(self)}
-        default_rng = default_values["mode"]
-        self.parameters = {
-            name: self._init_param(name, default_rng)
-            for name in param_names
-        }
+        default_ranges = {f.name: f.default for f in dataclasses.fields(self)}
+        default_range = default_ranges["mode"]
+        initializer = lambda PRNG_key, range_: jax.random.uniform(
+            PRNG_key,
+            shape=(self.n_modes, self.config.batch_size),
+            minval=range_.minimum,
+            maxval=range_.maximum
+        )
+        # Initialize the parameter
+        self._init_param("mode", default_range, initializer)
 
     def __call__(self):
-        # TODO: Refactor get all values in SynthModule
-        parameter_values = [p.from_0to1() for k, p in self.parameters.items()]
-        idx = jnp.argmax(parameter_values, axis=0)
-        return jax.nn.one_hot(idx, num_classes=len(parameter_values)).T
+        mode = from_0to1(self._mode, self._mode_range)
+        idx = jnp.argmax(mode, axis=0)
+        return jax.nn.one_hot(idx, num_classes=len(mode)).T
```

### Comparing `synthax-0.1.2/synthax/modules/control.py` & `synthax-0.2.0/synthax/modules/control.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,15 +33,14 @@
     Upsample control signals to the global sampling rate
 
     Uses linear interpolation to resample an input control signal to the
     audio buffer size set in config.
 
     Args:
         config (:class:`~synthax.config.SynthConfig`): Configuration.
-        PRNG_key (jax.random.PRNGKey): PRNG key already split.
     """
 
     def __call__(self, signal):
         def vmap_interp(s: Signal):
             return jnp.interp(
                 jnp.linspace(0, self.config.control_buffer_size, self.config.buffer_size),
                 jnp.linspace(0, self.config.control_buffer_size, self.config.control_buffer_size),
```

### Comparing `synthax-0.1.2/synthax/modules/envelopes.py` & `synthax-0.2.0/synthax/modules/envelopes.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,33 +18,33 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 import jax
 import jax.numpy as jnp
+import chex
 from synthax.modules.base import ControlRateModule
-from synthax.parameter import ModuleParameter, ModuleParameterRange
+from synthax.parameter import ModuleParameterRange, from_0to1
 from synthax.config import SynthConfig
 from synthax.types import ParameterSpec, Signal
 from typing import Optional
 
 
 class ADSR(ControlRateModule):
     """
     Envelope class for building a control-rate ADSR signal.
 
     Args:
         config (SynthConfig): See :class:`~synhtax.module.SynthModule`
-        PRNG_key (jax.random.PRNGKey): PRNG key already split.
-        attack (ParameterSpec): TODO
-        decay (ParameterSpec): TODO
-        sustain (ParameterSpec): TODO
-        release (ParameterSpec): TODO
-        alpha (ParameterSpec): TODO
+        attack (ParameterSpec): Accepts a parameter range, initial values or both.
+        decay (ParameterSpec): Accepts a parameter range, initial values or both.
+        sustain (ParameterSpec): Accepts a parameter range, initial values or both.
+        release (ParameterSpec): Accepts a parameter range, initial values or both.
+        alpha (ParameterSpec): Accepts a parameter range, initial values or both.
     """
 
     attack: Optional[ParameterSpec] = ModuleParameterRange(
         minimum=0.0,
         maximum=2.0,
         curve=0.5,
     )
@@ -86,50 +86,50 @@
             attack-and-decay (specifically, it will execute the entire attack,
             and only .25 seconds of the decay).
 
         If this is confusing, don't worry about it. ADSR's do a lot of work
         behind the scenes to make the playing experience feel natural.
 
         Args:
-            note_on_duration (TODO): Duration of note on event in seconds.
+            note_on_duration (chex.Array): Duration of note on event in seconds.
         """
 
-        # Calculations to accommodate attack/decay phase cut by note duration.
-        attack = self.parameters["attack"].from_0to1()
-        decay = self.parameters["decay"].from_0to1()
+        attack = from_0to1(self._attack, self._attack_range)
+        decay = from_0to1(self._decay, self._decay_range)
 
+        # Calculations to accommodate attack/decay phase cut by note duration.
         new_attack = jnp.minimum(attack, note_on_duration)
         new_decay = jnp.maximum(note_on_duration - attack, 0)
         new_decay = jnp.minimum(new_decay, decay)
 
         attack_signal = self.make_attack(new_attack)
         decay_signal = self.make_decay(new_attack, new_decay)
         release_signal = self.make_release(note_on_duration)
 
         signal = attack_signal * decay_signal * release_signal
 
         return signal
 
     def ramp(
             self,
-            duration: float,
-            start: Optional[float] = None,
+            duration: chex.Array,
+            start: Optional[chex.Array] = None,
             inverse: Optional[bool] = False
     ) -> Signal:
         """
         Makes a ramp of a given duration in seconds.
 
         The construction of this matrix is rather cryptic. Essentially, this
         method works by tilting and clipping ramps between 0 and 1, then
         applying a scaling factor :attr:`~alpha`.
 
         Args:
-            duration (TODO): Length of the ramp in seconds.
-            start (TODO): Initial delay of ramp in seconds.
-            inverse (TODO): Toggle to flip the ramp from ascending to descending.
+            duration (chex.Array): Length of the ramp in seconds.
+            start (chex.Array): Initial delay of ramp in seconds.
+            inverse (bool): Toggle to flip the ramp from ascending to descending.
         """
 
         duration = jnp.expand_dims(self.seconds_to_samples(duration), axis=1)
 
         # Convert to number of samples.
         if start is not None:
             start = jnp.expand_dims(self.seconds_to_samples(start), axis=1)
@@ -156,46 +156,49 @@
 
         if inverse:
             ramp = jnp.where(duration > 0.0, 1.0 - ramp, ramp)
 
         # Apply scaling factor.
         ramp = jnp.power(
             ramp,
-            jnp.expand_dims(self.parameters["alpha"].from_0to1(), axis=1)
+            jnp.expand_dims(from_0to1(self._alpha, self._alpha_range), axis=1)
         )
         return ramp
 
     def make_attack(self, attack_time) -> Signal:
         """
         Builds the attack portion of the envelope.
 
         Args:
-            attack_time (TODO): Length of the attack in seconds.
+            attack_time (chex.Array): Length of the attack in seconds.
         """
         return self.ramp(attack_time)
 
     def make_decay(self, attack_time, decay_time) -> Signal:
         """
         Creates the decay portion of the envelope.
 
         Args:
-            attack_time (TODO): Length of the attack in seconds.
-            decay_time (TODO): Length of the decay time in seconds.
+            attack_time (chex.Array): Length of the attack in seconds.
+            decay_time (chex.Array): Length of the decay time in seconds.
         """
-        sustain = jnp.expand_dims(self.parameters["sustain"].from_0to1(), axis=1)
+        sustain = jnp.expand_dims(
+            from_0to1(self._sustain, self._sustain_range),
+            axis=1
+        )
         a = 1.0 - sustain
         b = self.ramp(decay_time, start=attack_time, inverse=True)
         return jnp.squeeze(a * b + sustain)
 
     def make_release(self, note_on_duration) -> Signal:
         """
         Creates the release portion of the envelope.
 
         Args:
-            note_on_duration (TODO): Duration of midi note in seconds (release starts
+            note_on_duration (chex.Array): Duration of midi note in seconds (release starts
                 when the midi note is released).
         """
         return self.ramp(
-            self.parameters["release"].from_0to1(),
+            from_0to1(self._release, self._release_range),
             start=note_on_duration,
             inverse=True
         )
```

### Comparing `synthax-0.1.2/synthax/modules/filters.py` & `synthax-0.2.0/synthax/modules/filters.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,24 +23,22 @@
 import jax
 import jax.numpy as jnp
 from synthax.modules.base import SynthModule
 from synthax.types import Signal
 
 
 class LPF(SynthModule):
-    """Simple time-veritying low-pass filter.
+    """
+    Simple time-veritying low-pass filter.
 
-    Parameters:
+    Args:
         order (int): Order of the filter.
     """
     order: int
 
-    def setup(self):
-        super().setup()
-
     def __call__(self, audio_in: Signal, control_in: Signal):
         def tv_lpf(input_signal: Signal, input_control: Signal) -> Signal:
             dt = 1/self.config.sample_rate
             taus = 1.0 / (2 * jnp.pi * input_control)
 
             alphas = dt / (taus + dt)
 
@@ -54,8 +52,8 @@
             _, outputs = jax.lax.scan(
                 one_step,
                 state,
                 jnp.stack([alphas, input_signal], axis=-1)
             )
             return outputs[:, -1]
 
-        return jax.vmap(tv_lpf)(audio_in, control_in)
+        return jax.vmap(tv_lpf)(audio_in, control_in)
```

### Comparing `synthax-0.1.2/synthax/modules/keyboard.py` & `synthax-0.2.0/synthax/modules/keyboard.py`

 * *Files 15% similar despite different names*

```diff
@@ -19,38 +19,39 @@
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 import jax
 from flax import linen as nn
 from synthax.modules.base import ControlRateModule
-from synthax.parameter import ModuleParameter, ModuleParameterRange
+from synthax.parameter import ModuleParameterRange, from_0to1
 from synthax.config import SynthConfig
 from synthax.types import ParameterSpec
 from typing import Optional
 
 
 class MonophonicKeyboard(ControlRateModule):
     """
     A keyboard controller module. Mimics a mono-synth keyboard and contains
     parameters that output a midi_f0 and note duration.
 
     Args:
         config (:class:`~synthax.config.SynthConfig`): Configuration.
-        PRNG_key (jax.random.PRNGKey): PRNG key already split.
-        midi_f0 (ParameterSpec): TODO
-        duration (ParameterSpec): TODO
+        midi_f0 (ParameterSpec): Accepts a parameter range, initial values or both.
+        duration (ParameterSpec): Accepts a parameter range, initial values or both.
     """
 
     midi_f0: Optional[ParameterSpec] = ModuleParameterRange(
         minimum=0.0,
         maximum=127.0,
         curve=1.0,
     )
     duration: Optional[ParameterSpec] = ModuleParameterRange(
         minimum=0.01,
         maximum=4.0,
         curve=0.5,
     )
 
     def __call__(self):
-        return self.parameters["midi_f0"].from_0to1(), self.parameters["duration"].from_0to1()
+        midi_f0 = from_0to1(self._midi_f0, self._midi_f0_range)
+        duration = from_0to1(self._duration, self._duration_range)
+        return midi_f0, duration
```

### Comparing `synthax-0.1.2/synthax/modules/lfos.py` & `synthax-0.2.0/synthax/modules/lfos.py`

 * *Files 18% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 import jax
 import jax.numpy as jnp
 import chex
 from synthax.modules.base import ControlRateModule
-from synthax.parameter import ModuleParameter, ModuleParameterRange
+from synthax.parameter import ModuleParameterRange, from_0to1
 from synthax.config import SynthConfig
 from synthax.types import ParameterSpec, Signal
 from typing import Optional
 
 
 class LFO(ControlRateModule):
     """
@@ -36,40 +36,39 @@
 
     The LFO shape can be any mixture of sine, triangle, saw, reverse saw, and
     square waves. Contributions of each base-shape are determined by the
     :attr:`~synthax.module.LFO.lfo_types` values, which are between 0 and 1.
 
     Args:
         config (SynthConfig): See :class:`~synthax.module.SynthConfig`.
-        PRNG_key (jax.random.PRNGKey): PRNG key already split.
         exponent: A non-negative value that determines the discrimination of the
             soft-max selector for LFO shapes. Higher values will tend to favour
             one LFO shape over all others. Lower values will result in a more
             even blend of LFO shapes.
-        frequency (ParameterSpec): TODO
-        mod_depth (ParameterSpec): TODO
-        initial_phase (ParameterSpec): TODO
-        sin (ParameterSpec): TODO
-        tri (ParameterSpec): TODO
-        saw (ParameterSpec): TODO
-        rsaw (ParameterSpec): TODO
-        sqr (ParameterSpec): TODO
+        frequency (ParameterSpec): Accepts a parameter range, initial values or both.
+        mod_depth (ParameterSpec): Accepts a parameter range, initial values or both.
+        initial_phase (ParameterSpec): Accepts a parameter range, initial values or both.
+        sin (ParameterSpec): Accepts a parameter range, initial values or both.
+        tri (ParameterSpec): Accepts a parameter range, initial values or both.
+        saw (ParameterSpec): Accepts a parameter range, initial values or both.
+        rsaw (ParameterSpec): Accepts a parameter range, initial values or both.
+        sqr (ParameterSpec): Accepts a parameter range, initial values or both.
     """
 
     exponent: chex.Array = jnp.exp(1) # e
     frequency: Optional[ParameterSpec] = ModuleParameterRange(
         minimum=0.0,
         maximum=20.0,
         curve=0.25,
     )
     mod_depth: Optional[ParameterSpec] = ModuleParameterRange(
         minimum=-10.0,
         maximum=20.0,
         curve=0.5,
-        symmetric=True,
+        symmetric=True
     )
     initial_phase: Optional[ParameterSpec] = ModuleParameterRange(
         minimum=-jnp.pi,
         maximum=jnp.pi,
     )
     sin: Optional[ParameterSpec] = ModuleParameterRange(
         minimum=0.0,
@@ -90,38 +89,39 @@
     sqr: Optional[ParameterSpec] = ModuleParameterRange(
         minimum=0.0,
         maximum=1.0,
     )
 
     def setup(self):
         super().setup()
-        self.lfo_types = ["sin", "tri", "saw", "rsaw", "sqr"]
+        self.lfo_types = ["_sin", "_tri", "_saw", "_rsaw", "_sqr"]
 
     def __call__(self, mod_signal: Optional[Signal] = None):
         """
         Generates low frequency oscillator control signal.
 
         Args:
             mod_signal (Signal):  LFO rate modulation signal in Hz. To modulate the
                 depth of the LFO, use :class:`synthax.module.ControlRateVCA`.
         """
         # Create frequency signal
         frequency = self.make_control(mod_signal)
         argument = jnp.cumsum(2 * jnp.pi * frequency / self.control_rate, axis=1)
         argument += jnp.expand_dims(
-            self.parameters["initial_phase"].from_0to1(),
+            from_0to1(self._initial_phase, self._initial_phase_range),
             axis=1
         )
 
         # Get LFO shapes
         shapes = jnp.stack(self.make_lfo_shapes(argument), axis=1)
 
         # Apply mode selection to the LFO shapes
+        # TODO: avoid loop to improve jitted performance.
         mode = jnp.stack(
-            [self.parameters[lfo].from_0to1() for lfo in self.lfo_types],
+            [getattr(self, lfo) for lfo in self.lfo_types],
             axis=1
         )
         mode = jnp.power(mode, self.exponent)
         mode /= jnp.sum(mode, axis=1, keepdims=True)
 
         signal = jnp.matmul(jnp.expand_dims(mode, axis=1), shapes).squeeze(1)
         return signal
@@ -131,25 +131,26 @@
         Applies the LFO-rate modulation signal to the LFO base frequency.
 
         Args:
             mod_signal (Signal): Modulation signal in Hz. Positive values increase the
                 LFO base rate; negative values decrease it.
         """
         frequency = jnp.expand_dims(
-            self.parameters["frequency"].from_0to1(),
+            from_0to1(self._frequency, self._frequency_range),
             axis=1
         )
 
         # If no modulation, then return a view of the frequency of this
         # LFO expanded to the control buffer size
         if mod_signal is None:
             return jnp.broadcast_to(frequency, (frequency.shape[0], self.control_buffer_size))
 
         modulation = jnp.expand_dims(
-            self.parameters["mod_depth"].from_0to1(), axis=1
+            from_0to1(self._mod_depth, self._mod_depth_range),
+            axis=1
         ) * mod_signal
 
         return jnp.maximum(frequency + modulation, 0.0)
 
     def make_lfo_shapes(
         self,
         argument: Signal
```

### Comparing `synthax-0.1.2/synthax/modules/mixers.py` & `synthax-0.2.0/synthax/modules/mixers.py`

 * *Files 20% similar despite different names*

```diff
@@ -20,129 +20,110 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 import jax
 import jax.numpy as jnp
 import dataclasses
 from synthax.modules.base import SynthModule
-from synthax.parameter import ModuleParameter, ModuleParameterRange
-from synthax.config import SynthConfig
+from synthax.parameter import ModuleParameterRange, from_0to1
 from synthax.functional import normalize_if_clipping
 from synthax.types import Signal, ParameterSpec
 from typing import Optional
 
-
 class ModulationMixer(SynthModule):
     """
     A modulation matrix that combines :math:`N` input modulation signals to make
     :math:`M` output modulation signals. Each output is a linear combination of
     all in input signals, as determined by an :math:`N \times M` mixing matrix.
 
     Args:
         config (:class:`~synthax.config.SynthConfig`): Configuration.
-        PRNG_key (jax.random.PRNGKey): PRNG key already split.
         n_input (int): Number of input signals to module mix.
         n_output (int): Number of output signals to generate.
-        input_names (List(str)): TODO
-        output_names (List(str)): TODO
-        mod (ParameterSpec): TODO.
+        mod (ParameterSpec): Accepts a parameter range, initial values or both.
     """
 
     n_input: int
     n_output: int
-    input_names: Optional[list[str]] = None
-    output_names: Optional[list[str]] = None
     mod: Optional[ParameterSpec] = ModuleParameterRange(
         minimum=0.0,
         maximum=1.0,
-        curve=0.5,
+        curve=0.5
     )
 
     def setup(self):
-        param_names = []
-        for i in range(self.n_input):
-            for j in range(self.n_output):
-                # Apply custom param name if it was passed in
-                if self.input_names is not None:
-                    param_name = f"{self.input_names[i]}->{self.output_names[j]}"
-                else:
-                    param_name = f"{i}->{j}"
-                param_names.append(param_name)
-                setattr(self, param_name, self.mod)
-        # The default parameter range applies to all modes
-        default_values = {f.name: f.default for f in dataclasses.fields(self)}
-        default_rng = default_values["mod"]
-        self.parameters = {
-            name: self._init_param(name, default_rng)
-            for name in param_names
-        }
+        # The default parameter range applies to all inputs
+        default_ranges = {f.name: f.default for f in dataclasses.fields(self)}
+        default_range = default_ranges["mod"]
+        initializer = lambda PRNG_key, range_: jax.random.uniform(
+            PRNG_key,
+            shape=(self.config.batch_size, self.n_output, self.n_input),
+            minval=range_.minimum,
+            maxval=range_.maximum
+        )
+        # Initialize the parameter
+        self._init_param("mod", default_range, initializer)
 
     def __call__(self, *signals: Signal):
         """
         Performs mixture of modulation signals.
         """
 
-        parameter_values = jnp.array([p.from_0to1() for k, p in self.parameters.items()])
-        parameter_values = jnp.reshape(
-            parameter_values,
-            (self.batch_size, self.n_input, self.n_output)
-        )
-        parameter_values = jnp.swapaxes(parameter_values, 1, 2)
-
         signals = jnp.stack(signals, axis=1)
 
         modulation = jnp.array_split(
-            jnp.matmul(parameter_values, signals),
+            jnp.matmul(from_0to1(self._mod, self._mod_range), signals),
             self.n_output,
             axis=1
         )
+
+        # TODO: avoid loop to improve jitted performance.
         return tuple(m.squeeze(1) for m in modulation)
 
 
 class AudioMixer(SynthModule):
     """
     Sums together N audio signals and applies range-normalization if the
     resulting signal is outside of [-1, 1].
 
     Args:
         config (:class:`~synthax.config.SynthConfig`): Configuration.
-        PRNG_key (jax.random.PRNGKey): PRNG key already split.
-        n_input (int): TODO
-        names (List[str]): TODO
-        level (ParameterSpec): TODO
+        n_input (int): Number of inputs.
+        level (ParameterSpec): Accepts a parameter range, initial values or both, for all inputs equally.
     """
 
     n_input: int
-    names: Optional[list[str]] = None
     level: Optional[ParameterSpec] = ModuleParameterRange(
         minimum=0.0,
         maximum=1.0,
-        curve=1.0,
+        curve=1.0
     )
 
     def setup(self):
-        param_names = []
-        for i in range(self.n_input):
-            param_name = f"level{i}" if self.names is None else self.names[i]
-            param_names.append(param_name)
-            setattr(self, param_name, self.level)
-        # The default parameter range applies to all modes
-        default_values = {f.name: f.default for f in dataclasses.fields(self)}
-        default_rng = default_values["level"]
-        self.parameters = {
-            name: self._init_param(name, default_rng)
-            for name in param_names
-        }
+        # The default parameter range applies to all inputs
+        default_ranges = {f.name: f.default for f in dataclasses.fields(self)}
+        default_range = default_ranges["level"]
+        initializer = lambda PRNG_key, range_: jax.random.uniform(
+            PRNG_key,
+            shape=(self.config.batch_size, self.n_input),
+            minval=range_.minimum,
+            maxval=range_.maximum
+        )
+        # Initialize the parameter
+        self._init_param("level", default_range, initializer)
 
     def __call__(self, *signals: Signal):
         """
         Returns a mixed signal from an array of input signals.
         """
-        parameter_values = jnp.stack([p.from_0to1() for k, p in self.parameters.items()], axis=1)
+        # TODO: improve performance
         signals = jnp.stack(signals, axis=1)
+
+        # TODO: improve performance
         mixed_signal = normalize_if_clipping(
             jnp.matmul(
-                jnp.expand_dims(parameter_values, 1),
+                jnp.expand_dims(from_0to1(self._level, self._level_range), 1),
                 signals
             ).squeeze(1)
         )
+
         return mixed_signal
```

### Comparing `synthax-0.1.2/synthax/modules/oscillators.py` & `synthax-0.2.0/synthax/modules/oscillators.py`

 * *Files 14% similar despite different names*

```diff
@@ -20,47 +20,44 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 import jax
 import jax.numpy as jnp
 import chex
 from synthax.modules.base import SynthModule
-from synthax.parameter import ModuleParameter, ModuleParameterRange
+from synthax.parameter import ModuleParameterRange, from_0to1
 from synthax.config import SynthConfig
 from synthax.functional import midi_to_hz
 from synthax.types import Signal, ParameterSpec
 from typing import Optional
 
-
 class VCO(SynthModule):
     """
     Base class for voltage controlled oscillators.
 
     Think of this as a VCO on a modular synthesizer. It has a base pitch
     (specified here as a midi value), and a pitch modulation depth. Its call
     accepts a modulation signal between [-1, 1]. An array of 0's returns a
     stationary audio signal at its base pitch.
 
     Args:
-        config (SynthConfig): See :class:`~synhtax.module.SynthModule`
-        PRNG_key (jax.random.PRNGKey): PRNG key already split.
-        tuning (ParameterSpec): TODO
-        mod_depth (ParameterSpec): TODO
-        initial_phase (ParameterSpec): TODO
+        config (SynthConfig): See :class:`~synthax.module.SynthModule`
+        tuning (ParameterSpec): Accepts a parameter range, initial values or both.
+        mod_depth (ParameterSpec): Accepts a parameter range, initial values or both.
+        initial_phase (ParameterSpec): Accepts a parameter range, initial values or both.
     """
 
     tuning: Optional[ParameterSpec] = ModuleParameterRange(
         minimum=-24.0,
         maximum=24.0,
     )
     mod_depth: Optional[ParameterSpec] = ModuleParameterRange(
         minimum=-96.0,
         maximum=96.0,
-        curve=0.2,
-        symmetric=True,
+        curve=0.2
     )
     initial_phase: Optional[ParameterSpec] = ModuleParameterRange(
         minimum=-jnp.pi,
         maximum=jnp.pi,
     )
 
     def __call__(
@@ -68,97 +65,99 @@
         midi_f0: chex.Array,
         mod_signal: Optional[Signal] = None
     ) -> Signal:
         """
         Generates audio signal from modulation signal.
 
         Args:
-            midi_f0 (TODO): Fundamental of note in midi note value (0 - 127).
-            mod_signal (TODO): Modulation signal to apply to the pitch.
+            midi_f0 (chex.Array): Fundamental of note in midi note value (0 - 127).
+            mod_signal (synthax.types.Signal): Modulation signal to apply to the pitch.
         """
 
+        # TODO: improve performance
         control_as_frequency = self.make_control_as_frequency(midi_f0, mod_signal)
+        # TODO: improve performance
         cosine_argument = self.make_argument(control_as_frequency)
         cosine_argument += jnp.expand_dims(
-            self.parameters["initial_phase"].from_0to1(),
+            from_0to1(self._initial_phase, self._initial_phase_range),
             axis=1
         )
+        # TODO: improve performance
         signal = self.oscillator(cosine_argument, midi_f0)
         return signal
 
     def make_control_as_frequency(
         self,
         midi_f0: chex.Array,
         mod_signal: Optional[Signal] = None
     ) -> Signal:
         """
         Generates a time-varying control signal in frequency (Hz) from a midi
         fundamental pitch and pitch-modulation signal.
 
         Args:
-            midi_f0 (TODO): Fundamental pitch value in midi.
-            mod_signal (TODO): Pitch modulation signal in midi.
+            midi_f0 (chex.Array): Fundamental pitch value in midi.
+            mod_signal (synthax.types.Signal): Pitch modulation signal in midi.
         """
         midi_f0 = jnp.expand_dims(
-            midi_f0 + self.parameters["tuning"].from_0to1(),
+            midi_f0 + from_0to1(self._tuning, self._tuning_range),
             axis=1
         )
 
         # If there is no modulation, then convert the midi_f0 values to
         # frequency and return an expanded view that contains buffer size
         # number of values
         if mod_signal is None:
             control_hz = midi_to_hz(midi_f0)
             return jnp.broadcast_to(control_hz, (control_hz.shape[0], self.buffer_size))
 
         # If there is modulation, then add that to the fundamental,
         # clamp to a range [0.0, 127.0], then return in frequency Hz.
         modulation = jnp.expand_dims(
-            self.parameters["mod_depth"].from_0to1(),
+            from_0to1(self._mod_depth, self._mod_depth_range),
             axis=1
         ) * mod_signal
         control = jax.lax.clamp(0.0, midi_f0 + modulation, 127.0)
         return midi_to_hz(control)
 
     def make_argument(self, freq: Signal) -> Signal:
         """
         Generates the phase argument to feed an oscillating function to
         generate an audio signal.
 
         Args:
-            freq (TODO): Time-varying instantaneous frequency in Hz.
+            freq (synthax.types.Signal): Time-varying instantaneous frequency in Hz.
         """
         return jnp.cumsum(2 * jnp.pi * freq / self.sample_rate, axis=1)
 
     def oscillator(self, argument: Signal, *args: tuple, **kwargs: dict) -> Signal:
         """
         This function accepts a phase argument and generates output audio. It is
         implemented by the child class.
 
         Args:
-            argument (TODO): The phase of the oscillator at each time sample.
+            argument (synthax.types.Signal): The phase of the oscillator at each time sample.
         """
         raise NotImplementedError("Derived classes must override this method")
 
 
 class SineVCO(VCO):
     """
     Simple VCO that generates a pitched sinusoid.
 
     Args:
-        config (SynthConfig): See :class:`~synhtax.module.SynthModule`
-        PRNG_key (jax.random.PRNGKey): PRNG key already split.
+        config (SynthConfig): See :class:`~synthax.module.SynthModule`
     """
 
     def oscillator(self, argument: Signal, midi_f0: chex.Array) -> Signal:
         """
         A cosine oscillator.
 
         Args:
-            argument (TODO): The phase of the oscillator at each time sample.
+            argument (synthax.types.Signal): The phase of the oscillator at each time sample.
         """
         return jnp.cos(argument)
 
 
 class FmVCO(VCO):
     """
     Frequency modulation VCO. Takes a modulation signal as instantaneous
@@ -172,59 +171,58 @@
         :math:`I = \\Delta f / f_m`
 
     where :math:`I` is the modulation index, :math:`\\Delta f` is the frequency
     deviation imparted by the modulation, and :math:`f_m` is the modulation
     frequency, both in Hz.
 
     Args:
-        config (SynthConfig): See :class:`~synhtax.module.SynthModule`
-        PRNG_key (jax.random.PRNGKey): PRNG key already split.
+        config (SynthConfig): See :class:`~synthax.module.SynthModule`
     """
 
     # We include this override to output to make mod_signal non-optional
     def __call__(self, midi_f0: chex.Array, mod_signal: Signal) -> Signal:
         """
         Args:
-            midi_f0 (TODO): note value in midi
-            mod_signal (TODO): audio rate frequency modulation signal
+            midi_f0 (chex.Array): note value in midi
+            mod_signal (synthax.types.Signal): audio rate frequency modulation signal
         """
         return super().__call__(midi_f0, mod_signal)
 
     def make_control_as_frequency(
         self,
         midi_f0: chex.Array,
         mod_signal
     ) -> Signal:
         """
         Creates a time-varying control signal in instantaneous frequency (Hz).
 
         Args:
-            midi_f0 (TODO): Fundamental frequency in midi.
-            mod_signal (TODO): FM modulation signal (interpreted as modulation index).
+            midi_f0 (chex.Array): Fundamental frequency in midi.
+            mod_signal (synthax.types.Signal): FM modulation signal (interpreted as modulation index).
         """
         # Compute modulation in Hz space (rather than midi-space).
         f0_hz = jnp.expand_dims(
             midi_to_hz(
-                midi_f0 + self.parameters["tuning"].from_0to1()
+                midi_f0 + from_0to1(self._tuning, self._tuning_range),
             ),
             axis=1
         )
         fm_depth = jnp.expand_dims(
-            self.parameters["mod_depth"].from_0to1(),
+            from_0to1(self._mod_depth, self._mod_depth_range),
             axis=1
         ) * f0_hz
         modulation_hz = fm_depth * mod_signal
         return jax.lax.clamp(0.0, f0_hz + modulation_hz, self.nyquist)
 
     def oscillator(self, argument: Signal, midi_f0: chex.Array) -> Signal:
         """
         A cosine oscillator. ...Good ol' cosine.
 
         Args:
-            argument (TODO): The phase of the oscillator at each time sample.
+            argument (synthax.types.Signal): The phase of the oscillator at each time sample.
         """
         return jnp.cos(argument)
 
 
 class SquareSawVCO(VCO):
     """
     An oscillator that can take on either a square or a sawtooth waveshape, and
@@ -234,31 +232,29 @@
 
     With apologies to Lazzarini and Timoney (2010).
     `"New perspectives on distortion synthesis for virtual analog oscillators."
     <https://doi.org/10.1162/comj.2010.34.1.28>`_
     Computer Music Journal 34, no. 1: 28-40.
 
     Args:
-        config (SynthConfig): See :class:`~synhtax.module.SynthModule`
-        PRNG_key (jax.random.PRNGKey): PRNG key already split.
-        tuning (ParameterSpec): TODO
-        mod_depth (ParameterSpec): TODO
-        initial_phase (ParameterSpec): TODO
-        shape (ParameterSpec): TODO
+        config (SynthConfig): See :class:`~synthax.module.SynthModule`
+        tuning (ParameterSpec): Accepts a parameter range, initial values or both.
+        mod_depth (ParameterSpec): Accepts a parameter range, initial values or both.
+        initial_phase (ParameterSpec): Accepts a parameter range, initial values or both.
+        shape (ParameterSpec): Accepts a parameter range, initial values or both.
     """
 
     tuning: Optional[ParameterSpec] = ModuleParameterRange(
         minimum=-24.0,
         maximum=24.0,
     )
     mod_depth: Optional[ParameterSpec] = ModuleParameterRange(
         minimum=-96.0,
         maximum=96.0,
-        curve=0.2,
-        symmetric=True,
+        curve=0.2
     )
     initial_phase: Optional[ParameterSpec] = ModuleParameterRange(
         minimum=-jnp.pi,
         maximum=jnp.pi,
     )
     shape: Optional[ParameterSpec] = ModuleParameterRange(
         minimum=0.0,
@@ -266,78 +262,69 @@
     )
 
     def oscillator(self, argument: Signal, midi_f0: chex.Array) -> Signal:
         """
         Generates output square/saw audio given a phase argument.
 
         Args:
-            argument (TODO): The phase of the oscillator at each time sample.
-            midi_f0 (TODO): Fundamental frequency in midi.
+            argument (synthax.types.Signal): The phase of the oscillator at each time sample.
+            midi_f0 (chex.Array): Fundamental frequency in midi.
         """
         partials = jnp.expand_dims(self.partials_constant(midi_f0), axis=1)
         square = jnp.tanh(jnp.pi * partials * jnp.sin(argument) / 2)
-        shape = jnp.expand_dims(self.parameters["shape"].from_0to1(), axis=1)
+        shape = jnp.expand_dims(
+            from_0to1(self._shape, self._shape_range),
+            axis=1
+        )
         return (1 - shape / 2) * square * (1 + shape * jnp.cos(argument))
 
     def partials_constant(self, midi_f0):
         """
         Calculates a value to determine the number of overtones in the resulting
         square / saw wave, in order to keep aliasing at an acceptable level.
         Higher fundamental frequencies require fewer partials for a rich sound;
         lower-frequency sounds can safely have more partials without causing
         audible aliasing.
 
         Args:
-            midi_f0 (TODO): Fundamental frequency in midi.
+            midi_f0 (chex.Array): Fundamental frequency in midi.
         """
+        tuning = from_0to1(self._tuning, self._tuning_range)
+        mod_depth = from_0to1(self._mod_depth, self._mod_depth_range)
+
         max_pitch = (
-            midi_f0 + self.parameters["tuning"].from_0to1() + jnp.maximum(self.parameters["mod_depth"].from_0to1(), 0)
+            midi_f0 + tuning + jnp.maximum(mod_depth, 0)
         )
         max_f0 = midi_to_hz(max_pitch)
         return 12000 / (max_f0 * jnp.log10(max_f0))
 
 
 class Noise(SynthModule):
     """
     Generates white noise that is the same length as the buffer.
 
-    TODO:
-
-    For performance noise is pre-computed. In order to maintain
-    reproducibility noise must be computed on the CPU and then transferred
-    to the GPU, if a GPU is being used. We pre-compute
-    :attr:`~synthax.config.BASE_REPRODUCIBLE_BATCH_SIZE`
-    samples of noise and then repeat those for larger batch sizes.
-
-    To keep things fast we only support multiples of
-    :attr:`~synthax.config.BASE_REPRODUCIBLE_BATCH_SIZE`
-    when reproducibility mode is enabled. For example, if you batch size
-    is 4 times :attr:`~synthax.config.BASE_REPRODUCIBLE_BATCH_SIZE`, then
-    you get the same noise signals repeated 4 times.
-
     `Note`: If you have multiple `Noise` modules in the same
     :class:`~synthax.synth.BaseSynth`, make sure you instantiate
     each `Noise` with a unique seed.
 
     Args:
-        config (SynthConfig): See :class:`~synhtax.module.SynthModule`
-        PRNG_key (jax.random.PRNGKey): PRNG key already split.
+        config (SynthConfig): See :class:`~synthax.module.SynthModule`
+        seed (int): Seed for the random number generator.
     """
 
+    seed: int = 0
+
     def setup(self):
         def make_noise():
             return jnp.broadcast_to(
                 jax.random.uniform(
-                    self.PRNG_key,
+                    jax.random.PRNGKey(self.seed),
                     shape=(1, self.buffer_size),
                     minval=-1.0,
                     maxval=1.0
                 ),
                 (self.batch_size, self.buffer_size)
             )
-        self.parameters = {
-            "noise": make_noise()
-        }
+        self._noise = make_noise()
 
     def __call__(self) -> Signal:
-        signal = self.parameters["noise"]
-        return signal
+        return self._noise
```

### Comparing `synthax-0.1.2/synthax/parameter.py` & `synthax-0.2.0/synthax/parameter.py`

 * *Files 16% similar despite different names*

```diff
@@ -22,18 +22,17 @@
 
 """
 Parameters for DDSP Modules
 """
 
 import jax
 import chex
-from flax import linen as nn
-from flax import struct
 import jax.numpy as jnp
-from typing import Callable, NamedTuple
+from flax import struct
+from typing import NamedTuple
 
 @struct.dataclass
 class ModuleParameterRange:
     """
     `ModuleParameterRange` class is a structure for keeping track of
     the specific range that a parameter might take on. Also handles
     functionality for converting between machine-readable range [0, 1] and a
@@ -49,88 +48,85 @@
         symmetric (bool): whether or not the parameter range is symmetric,
             allows for curves around a center point. When this is True,
             a curve value of one is linear, greater than one emphasizes
             the minimum and maximum, and less than one emphasizes values
             closer to :math:`(maximum - minimum)/2`.
     """
 
-    minimum: float
-    maximum: float
-    curve: float = 1.0
+    minimum: jax.typing.ArrayLike
+    maximum: jax.typing.ArrayLike
+    curve: jax.typing.ArrayLike = 1.0
     symmetric: bool = False
 
 
-def from_0to1(normalized: jax.typing.ArrayLike, range: ModuleParameterRange) -> jax.typing.ArrayLike:
-    """
-    Set value of this parameter using a normalized value in the range [0,1]
+class ModuleParameterSpec(NamedTuple):
+    range_: ModuleParameterRange
+    value: jax.typing.ArrayLike
 
-    Args:
-        normalized (float): value within machine-readable range [0, 1] to convert to
-            human-readable range [minimum, maximum].
-    """
-    if not range.symmetric:
-        if range.curve != 1.0:
-            normalized = jnp.exp2(jnp.log2(normalized) / range.curve)
 
-        return range.minimum + (range.maximum - range.minimum) * normalized
+def apply_asymmetricfrom(
+    normalized: jax.typing.ArrayLike,
+    curve: jax.typing.ArrayLike,
+    range: ModuleParameterRange
+) -> jax.typing.ArrayLike:
+    apply_curve = lambda normalized, curve: jnp.exp2(jnp.log2(normalized) / curve)
+    normalized = jax.lax.cond(curve, apply_curve, lambda x, _: x, normalized, range.curve)
+    return range.minimum + (range.maximum - range.minimum) * normalized
 
-    # Compute the curve for a symmetric curve
-    dist = 2.0 * normalized - 1.0
-    if range.curve != 1.0:
-        normalized = jnp.where(
-            dist == 0.0,
-            dist,
-            jnp.exp2(jnp.log2(jnp.abs(dist)) / range.curve) * jnp.sign(dist),
-        )
 
+def apply_symmetricfrom(
+    normalized: jax.typing.ArrayLike,
+    curve: jax.typing.ArrayLike,
+    range: ModuleParameterRange
+) -> jax.typing.ArrayLike:
+    dist = 2.0 * normalized - 1.0
+    apply_curve = lambda dist, curve: jnp.where(
+        dist == 0.0,
+        dist,
+        jnp.exp2(jnp.log2(jnp.abs(dist)) / curve) * jnp.sign(dist)
+    )
+    normalized = jax.lax.cond(curve, apply_curve, lambda x, _: x, dist, range.curve)
     return range.minimum + (range.maximum - range.minimum) / 2.0 * (normalized + 1.0)
 
 
-def to_0to1(value: jax.typing.ArrayLike, range: ModuleParameterRange) -> jax.typing.ArrayLike:
-    """
-    Convert from human-readable range [minimum, maximum] to machine-range [0, 1].
+def apply_asynmetricto(normalized: jax.typing.ArrayLike,
+    curve: jax.typing.ArrayLike,
+    range: ModuleParameterRange
+) -> jax.typing.ArrayLike:
+    apply_curve = lambda normalized, curve: jnp.power(normalized, curve)
+    normalized = jax.lax.cond(curve, apply_curve, lambda x, _: x, normalized, range.curve)
+    return normalized
+
+def apply_symmetricto(
+    normalized: jax.typing.ArrayLike,
+    curve: jax.typing.ArrayLike,
+    range: ModuleParameterRange
+) -> jax.typing.ArrayLike:
+    dist = 2.0 * normalized - 1.0
+    apply_curve = lambda dist, curve: (1.0 + jnp.power(jnp.abs(dist), curve) * jnp.sign(dist)) / 2.0
+    normalized = jax.lax.cond(curve, apply_curve, lambda x, _: x, dist, range.curve)
+    return normalized
 
+
+def from_0to1(normalized: chex.Array, range: ModuleParameterRange) -> jax.typing.ArrayLike:
+    """
+    Set value of this parameter using a normalized value in the range [0,1]
     Args:
-        value (chex.Array): value within the range defined by minimum and maximum
+        normalized (chex.Array): value within machine-readable range [0, 1] to convert to
+            human-readable range [minimum, maximum].
     """
-    normalized = (value - range.minimum) / (range.maximum - range.minimum)
-
-    if not range.symmetric:
-        if range.curve != 1:
-            normalized = jnp.power(normalized, range.curve)
-        return normalized
+    curve = jnp.all(range.curve  == 1)
 
-    dist = 2.0 * normalized - 1.0
-    return (1.0 + jnp.power(jnp.abs(dist), range.curve) * jnp.sign(dist)) / 2.0
+    return jax.lax.cond(range.symmetric, apply_symmetricfrom, apply_asymmetricfrom, normalized, curve, range)
 
 
-class ModuleParameterSpec(NamedTuple):
-    range: ModuleParameterRange
-    value: jax.typing.ArrayLike
-
-class ModuleParameter(nn.Module):
+def to_0to1(value: chex.Array, range: ModuleParameterRange) -> jax.typing.ArrayLike:
     """
+    Convert from human-readable range [minimum, maximum] to machine-range [0, 1].
     Args:
-        name (str): A name for this parameter
-        range (ModuleParameterRange): Object that supports conversion
-            between human-readable range and machine-readable [0,1] range.
-        value (chex.Array): initial value of this parameter in the human-readable range.
+        value (chex.Array): value within the range defined by minimum and maximum
     """
+    normalized = (value - range.minimum) / (range.maximum - range.minimum)
 
-    name: str
-    range: ModuleParameterRange
-    value: chex.Array
-
-    def setup(self):
-        self._value = self.param(
-            self.name,
-            lambda _: self.value
-        )
-
-    def from_0to1(self) -> chex.Array:
-        """
-        Get the value of this parameter in the human-readable range.
-        """
-        return from_0to1(self._value, self.range)
+    curve = jnp.all(range.curve  == 1)
 
-    def __repr__(self):
-        return f"ModuleParameter({self.__dict__})"
+    return jax.lax.cond(range.symmetric, apply_symmetricto, apply_asynmetricto, normalized, curve, range)
```

### Comparing `synthax-0.1.2/synthax/synth.py` & `synthax-0.2.0/synthax/synth.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,20 +20,19 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 """
 :class:`~synthax.module.SynthModule` wired together form a modular synthesizer.
 """
 
-import os
-import yaml
-import jax
+import jax.numpy as jnp
 import chex
 from flax import linen as nn
 from synthax.config import SynthConfig
+from synthax.parameter import ModuleParameterRange
 
 from synthax.modules.oscillators import SineVCO, FmVCO, SquareSawVCO, Noise
 from synthax.modules.envelopes import ADSR
 from synthax.modules.lfos import LFO
 from synthax.modules.amplifiers import VCA, ControlRateVCA
 from synthax.modules.mixers import AudioMixer, ModulationMixer
 from synthax.modules.control import ControlRateUpsample
@@ -43,19 +42,17 @@
 class BaseSynth(nn.Module):
     """
     Base class for synthesizers that combine one or more
     :class:`~synthax.module.SynthModule` to create a full synth
     architecture.
 
     Args:
-        PRNG_key (jax.random.PRNGKey): PRNG key already split.
         config (:class:`~synthax.config.SynthConfig`): Global configuration.
     """
 
-    PRNG_key: jax.random.PRNGKey
     config: SynthConfig
 
 
     def setup(self):
         """
         Each `BaseSynth` should override this.
         """
@@ -99,15 +96,14 @@
     :class:`~synthax.module.ModulationMixer` and an
     :class:`~synthax.module.AudioMixer`. Modulation signals
     generated from control modules (:class:`~synthax.module.ADSR`
     and :class:`~synthax.module.LFO`) are upsampled to the audio
     sample rate before being passed to audio rate modules.
 
     Args:
-        PRNG_key (jax.random.PRNGKey): PRNG key already split.
         config (:class:`~synthax.config.SynthConfig`): Global configuration.
     """
 
     def setup(self):
         # Define modules
         modules_spec = [
             ("keyboard", MonophonicKeyboard, {}),
@@ -123,51 +119,31 @@
             ("lfo_1_rate_adsr", ADSR, {}),
             ("lfo_2_rate_adsr", ADSR, {}),
             ("lfo_3_rate_adsr", ADSR, {}),
             ("control_vca", ControlRateVCA, {}),
             ("control_upsample", ControlRateUpsample, {}),
             ("mod_matrix", ModulationMixer, {
                 "n_input": 6,
-                "n_output": 7,
-                "input_names": [
-                    "adsr_1",
-                    "adsr_2",
-                    "adsr_3",
-                    "lfo_1",
-                    "lfo_2",
-                    "lfo_3"
-                ],
-                "output_names": [
-                    "vco_1_pitch",
-                    "vco_1_amp",
-                    "vco_2_pitch",
-                    "vco_2_amp",
-                    "vco_3_pitch",
-                    "vco_3_amp",
-                    "noise_amp",
-                ]
+                "n_output": 7
             }
             ),
             ("vco_1", SineVCO, {}),
             ("vco_2", SquareSawVCO, {}),
             ("vco_3", SineVCO, {}),
             ("vco_4", FmVCO, {}),
             ("noise", Noise, {}),
             ("vca", VCA, {}),
             ("mixer", AudioMixer, {
                 "n_input": 4,
-                "names": ["vco_1", "vco_2", "vco_4", "noise"]
             })
         ]
 
-        key = self.PRNG_key
         modules = {}
         for name, module, params in modules_spec:
-            key, subkey = jax.random.split(key)
-            modules[name] = module(PRNG_key=subkey, config=self.config, **params)
+            modules[name] = module(config=self.config, **params)
 
         self.modules = modules
 
     def __call__(self, *args, **kwargs) -> chex.Array:
         # The convention for triggering a note event is that it has
         # the same note_on_duration for both ADSRs.
         midi_f0, note_on_duration = self.modules["keyboard"]()
@@ -236,15 +212,14 @@
     :class:`~synthax.module.ModulationMixer` and an
     :class:`~synthax.module.AudioMixer`. Modulation signals
     generated from control modules (:class:`~synthax.module.ADSR`
     and :class:`~synthax.module.LFO`) are upsampled to the audio
     sample rate before being passed to audio rate modules.
 
     Args:
-        PRNG_key (jax.random.PRNGKey): PRNG key already split.
         config (:class:`~synthax.config.SynthConfig`): Global configuration.
     """
 
     def setup(self):
         # Define modules
         modules_spec = [
             ("keyboard", MonophonicKeyboard, {}),
@@ -256,45 +231,34 @@
             ("lfo_2_amp_adsr", ADSR, {}),
             ("lfo_1_rate_adsr", ADSR, {}),
             ("lfo_2_rate_adsr", ADSR, {}),
             ("control_vca", ControlRateVCA, {}),
             ("control_upsample", ControlRateUpsample, {}),
             ("mod_matrix", ModulationMixer, {
                 "n_input": 4,
-                "n_output": 5,
-                "input_names": [
-                    "adsr_1",
-                    "adsr_2",
-                    "lfo_1",
-                    "lfo_2",
-                ],
-                "output_names": [
-                    "vco_1_pitch",
-                    "vco_1_amp",
-                    "vco_2_pitch",
-                    "vco_2_amp",
-                    "noise_amp",
-                ]
+                "n_output": 5
             }
             ),
             ("vco_1", SineVCO, {}),
             ("vco_2", SquareSawVCO, {}),
             ("noise", Noise, {}),
             ("vca", VCA, {}),
             ("mixer", AudioMixer, {
                 "n_input": 3,
-                "names": ["vco_1", "vco_2", "noise"]
+                "level": ModuleParameterRange(
+                    minimum=0,
+                    maximum=1,
+                    curve=jnp.array([1, 1, 0.025]) # 0.025 is for noise
+                )
             })
         ]
 
-        key = self.PRNG_key
         modules = {}
         for name, module, params in modules_spec:
-            key, subkey = jax.random.split(key)
-            modules[name] = module(PRNG_key=subkey, config=self.config, **params)
+            modules[name] = module(config=self.config, **params)
 
         self.modules = modules
 
     def __call__(self, *args, **kwargs) -> chex.Array:
         # The convention for triggering a note event is that it has
         # the same note_on_duration for both ADSRs.
         midi_f0, note_on_duration = self.modules["keyboard"]()
@@ -337,15 +301,14 @@
         return self.modules["mixer"](vco_1_out, vco_2_out, noise_out)
 
 class ParametricSynth(BaseSynth):
     """
     Define a synthesizer given the number of VCOs by type.
 
     Args:
-        PRNG_key (jax.random.PRNGKey): PRNG key already split.
         config (:class:`~synthax.config.SynthConfig`): Global configuration.
         sine (int): Number of :class:`~synthax.modules.oscillators.SineVCO`
         square_saw (int): Number of :class:`~synthax.modules.oscillators.SquareSawVCO`
         fm_sine (int): Number of :class:`~synthax.modules.oscillators.FmVCO` and
             :class:`~synthax.modules.oscillators.SineVCO`
         fm_square_saw (int): Number of :class:`~synthax.modules.oscillators.FmVCO` and
             :class:`~synthax.modules.oscillators.SquareSawVCO`
@@ -422,38 +385,33 @@
         # Modulation mixer
         modules_spec.append(
             (
                 "mod_matrix",
                 ModulationMixer,
                 {
                     "n_input": len(mod_input),
-                    "n_output": len(mod_output) + 1,
-                    "input_names": mod_input,
-                    "output_names": mod_output + ["noise_amp"],
+                    "n_output": len(mod_output) + 1
                 },
              )
         )
 
         # Audio mixer
         modules_spec.append(
             (
                 "mixer",
                 AudioMixer,
                 {
                     "n_input": len(mixable_vcos) + 1, # VCOs + noise
-                    "names": mixable_vcos + ["noise"],
                 },
             )
         )
 
-        key = self.PRNG_key
         modules = {}
         for name, module, params in modules_spec:
-            key, subkey = jax.random.split(key)
-            modules[name] = module(PRNG_key=subkey, config=self.config, **params)
+            modules[name] = module(config=self.config, **params)
 
         self.modules = modules
 
     def __call__(self, *args, **kwargs) -> chex.Array:
         # Keyboard for each VCO
         keyboards = [] # [(midi_f0, note_on_duration)]
         for i in range(1, self.n + 1):
```

### Comparing `synthax-0.1.2/synthax/types.py` & `synthax-0.2.0/synthax/types.py`

 * *Files identical despite different names*

### Comparing `synthax-0.1.2/synthax.egg-info/PKG-INFO` & `synthax-0.2.0/synthax.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: synthax
-Version: 0.1.2
+Version: 0.2.0
 Summary: SynthAX: A Fast Modular Synthesizer in JAX
 Home-page: https://github.com/PapayaResearch/synthax
 Author: Manuel Cherep, Nikhil Singh
 Author-email: mcherep@mit.edu, nsingh1@mit.edu
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -28,35 +28,32 @@
 
 ```python
 import jax
 from synthax.config import SynthConfig
 from synthax.synth import ParametricSynth
 
 # Generate PRNG key
-key = jax.random.PRNGKey(42)
 config = SynthConfig(
     batch_size=16,
     sample_rate=44100,
     buffer_size_seconds=4.0
 )
 
-key, subkey = jax.random.split(key)
 # Instantiate synthesizer
 synth = ParametricSynth(
-    PRNG_key=subkey,
     config=config,
     sine=1,
     square_saw=1,
     fm_sine=1,
     fm_square_saw=0
 )
 
-key, subkey = jax.random.split(key)
 # Initialize and run
-params = synth.init(subkey)
+key = jax.random.PRNGKey(42)
+params = synth.init(key)
 audio = jax.jit(synth.apply)(params)
 ```
 
 ## Installation
 
 The latest `synthax` release can directly be installed from PyPI:
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: synthax Version: 0.1.2 Summary: SynthAX: A Fast
+Metadata-Version: 2.1 Name: synthax Version: 0.2.0 Summary: SynthAX: A Fast
 Modular Synthesizer in JAX Home-page: https://github.com/PapayaResearch/synthax
 Author: Manuel Cherep, Nikhil Singh Author-email: mcherep@mit.edu,
 nsingh1@mit.edu Classifier: Programming Language :: Python :: 3.9 Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
 Independent Requires-Python: >=3.9 Description-Content-Type: text/markdown
 License-File: LICENSE # SynthAX: A Fast Modular Synthesizer in JAX â¡ï¸ [!
 [Pyversions](https://img.shields.io/pypi/pyversions/synthax.svg?style=flat-
@@ -17,25 +17,23 @@
 audio over 60,000 times faster than realtime, and significantly faster than the
 state-of-the-art in accelerated sound synthesis. It leverages massive
 vectorization and high-throughput accelerators. You can get started here [!
 [Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://
 colab.research.google.com/github/PapayaResearch/synthax/blob/main/examples/
 walkthrough.ipynb) ## Basic `synthax` API Usage ```python import jax from
 synthax.config import SynthConfig from synthax.synth import ParametricSynth #
-Generate PRNG key key = jax.random.PRNGKey(42) config = SynthConfig
-( batch_size=16, sample_rate=44100, buffer_size_seconds=4.0 ) key, subkey =
-jax.random.split(key) # Instantiate synthesizer synth = ParametricSynth
-( PRNG_key=subkey, config=config, sine=1, square_saw=1, fm_sine=1,
-fm_square_saw=0 ) key, subkey = jax.random.split(key) # Initialize and run
-params = synth.init(subkey) audio = jax.jit(synth.apply)(params) ``` ##
-Installation The latest `synthax` release can directly be installed from PyPI:
-``` pip install synthax ``` If you want to get the most recent commit, please
-install directly from the repository: ``` pip install git+https://github.com/
-PapayaResearch/synthax.git@main ``` In order to use JAX on your accelerators,
-you can find more details in the [JAX documentation](https://github.com/google/
-jax#installation). ## Acknowledgements & Citing If you use `synthax` in your
-research, please cite the following: ``` @software{synthax2023, author =
-{Cherep, Manuel and Singh, Nikhil}, title = {SynthAX: A Fast Modular
-Synthesizer in JAX}, url = {https://github.com/PapayaResearch/synthax}, version
-= {0.1.0}, year = {2023}, } ``` This project is based on [torchsynth](https://
-github.com/torchsynth/torchsynth). We acknowledge financial support by
-Fulbright Spain.
+Generate PRNG key config = SynthConfig( batch_size=16, sample_rate=44100,
+buffer_size_seconds=4.0 ) # Instantiate synthesizer synth = ParametricSynth
+( config=config, sine=1, square_saw=1, fm_sine=1, fm_square_saw=0 ) #
+Initialize and run key = jax.random.PRNGKey(42) params = synth.init(key) audio
+= jax.jit(synth.apply)(params) ``` ## Installation The latest `synthax` release
+can directly be installed from PyPI: ``` pip install synthax ``` If you want to
+get the most recent commit, please install directly from the repository: ```
+pip install git+https://github.com/PapayaResearch/synthax.git@main ``` In order
+to use JAX on your accelerators, you can find more details in the [JAX
+documentation](https://github.com/google/jax#installation). ## Acknowledgements
+& Citing If you use `synthax` in your research, please cite the following: ```
+@software{synthax2023, author = {Cherep, Manuel and Singh, Nikhil}, title =
+{SynthAX: A Fast Modular Synthesizer in JAX}, url = {https://github.com/
+PapayaResearch/synthax}, version = {0.1.0}, year = {2023}, } ``` This project
+is based on [torchsynth](https://github.com/torchsynth/torchsynth). We
+acknowledge financial support by Fulbright Spain.
```

### Comparing `synthax-0.1.2/synthax.egg-info/SOURCES.txt` & `synthax-0.2.0/synthax.egg-info/SOURCES.txt`

 * *Files identical despite different names*

