# Comparing `tmp/audio_separator-0.2.3.tar.gz` & `tmp/audio_separator-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audio_separator-0.2.3.tar", max compression
+gzip compressed data, was "audio_separator-0.3.1.tar", max compression
```

## Comparing `audio_separator-0.2.3.tar` & `audio_separator-0.3.1.tar`

### file list

```diff
@@ -1,10 +1,9 @@
--rw-r--r--   0        0        0     1069 2023-06-30 05:57:58.913442 audio_separator-0.2.3/LICENSE
--rw-r--r--   0        0        0     6469 2023-06-30 22:31:30.149482 audio_separator-0.2.3/README.md
--rw-r--r--   0        0        0       33 2023-06-30 18:38:54.200542 audio_separator-0.2.3/audio_separator/__init__.py
--rw-r--r--   0        0        0    11008 2023-06-30 22:48:43.228969 audio_separator-0.2.3/audio_separator/separator.py
--rw-r--r--   0        0        0        0 2023-06-30 05:58:37.414385 audio_separator-0.2.3/audio_separator/utils/__init__.py
--rwxr-xr-x   0        0        0     1726 2023-06-30 22:48:43.140580 audio_separator-0.2.3/audio_separator/utils/cli.py
--rw-r--r--   0        0        0     2041 2023-06-30 22:48:43.147133 audio_separator-0.2.3/audio_separator/utils/pyrb.py
--rw-r--r--   0        0        0    24722 2023-06-30 22:48:43.362641 audio_separator-0.2.3/audio_separator/utils/spec_utils.py
--rw-r--r--   0        0        0      760 2023-06-30 22:50:14.138142 audio_separator-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     7290 1970-01-01 00:00:00.000000 audio_separator-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-06-30 05:57:58.913442 audio_separator-0.3.1/LICENSE
+-rw-r--r--   0        0        0     6659 2023-07-02 02:44:13.948375 audio_separator-0.3.1/README.md
+-rw-r--r--   0        0        0       33 2023-06-30 18:38:54.200542 audio_separator-0.3.1/audio_separator/__init__.py
+-rw-r--r--   0        0        0    11878 2023-07-07 18:49:58.574514 audio_separator-0.3.1/audio_separator/separator.py
+-rw-r--r--   0        0        0        0 2023-06-30 05:58:37.414385 audio_separator-0.3.1/audio_separator/utils/__init__.py
+-rwxr-xr-x   0        0        0     2241 2023-07-07 19:01:19.825510 audio_separator-0.3.1/audio_separator/utils/cli.py
+-rw-r--r--   0        0        0    21906 2023-07-07 18:41:58.680039 audio_separator-0.3.1/audio_separator/utils/spec_utils.py
+-rw-r--r--   0        0        0      760 2023-07-07 17:27:08.214286 audio_separator-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     7480 1970-01-01 00:00:00.000000 audio_separator-0.3.1/PKG-INFO
```

### Comparing `audio_separator-0.2.3/LICENSE` & `audio_separator-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `audio_separator-0.2.3/README.md` & `audio_separator-0.3.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Audio Separator
+# Audio Separator 🎶
 
 [![PyPI version](https://badge.fury.io/py/audio-separator.svg)](https://badge.fury.io/py/audio-separator)
 
 Summary: Easy to use vocal separation on CLI or as a python package, using the amazing MDX-Net models from UVR trained by @Anjok07
 
 Audio Separator is a Python package that allows you to separate an audio file into two stems, primary and secondary, using a model in the ONNX format trained by @Anjok07 for use with UVR (https://github.com/Anjok07/ultimatevocalremovergui).
 
@@ -12,22 +12,22 @@
 
 - Separate audio into instrumental and vocal stems.
 - Supports all common audio formats (WAV, MP3, FLAC, M4A, etc.)
 - Ability to specify a pre-trained deep learning model in ONNX format.
 - CLI support for easy use in scripts and batch processing.
 - Python API for integration into other projects.
 
-## Installation
+## Installation 🛠️
 
 You can install Audio Separator using pip:
 
 `pip install audio-separator`
 
 
-## Usage
+## Usage 🚀
 
 ### Command Line Interface (CLI)
 
 You can use Audio Separator via the command line:
 
 ```sh
 audio-separator [audio_file] --model_name [model_name]
@@ -66,15 +66,15 @@
 ## Parameters for the Separator class
 
 - audio_file: The path to the audio file to be separated. Supports all common formats (WAV, MP3, FLAC, M4A, etc.)
 - model_name: (Optional) The name of the model to use for separation. Defaults to 'UVR_MDXNET_KARA_2', a very powerful model for Karaoke instrumental tracks.
 - model_file_dir: (Optional) Directory to cache model files in. Default: /tmp/audio-separator-models/
 - output_dir: (Optional) Directory where the separated files will be saved. If not specified, outputs to current dir.
 
-## Requirements
+## Requirements 📋
 
 Python <= 3.10 (one of the dependencies doesn't like 3.11 yet)
 
 Libraries: onnx, onnxruntime, numpy, soundfile, librosa, torch, wget, six
 
 ## Developing Locally
 
@@ -134,28 +134,32 @@
 
 ```
 poetry build
 ```
 
 This will generate the distribution packages in the dist directory - but for now only @beveradb will be able to publish to PyPI.
 
-## Contributing
+## Contributing 🤝
 
 Contributions are very much welcome! Please fork the repository and submit a pull request with your changes, and I'll try to review, merge and publish promptly!
 
 - This project is 100% open-source and free for anyone to use and modify as they wish. 
 - If the maintenance workload for this repo somehow becomes too much for me I'll ask for volunteers to share maintainership of the repo, though I don't think that is very likely
 - Development and support for the MDX-Net separation models is part of the main [UVR project](https://github.com/Anjok07/ultimatevocalremovergui), this repo is just a CLI/Python package wrapper to simplify running those models programmatically. So, if you want to try and improve the actual models, please get involved in the UVR project and look for guidance there!
 
-## License
+## License 📄
 
 This project is licensed under the MIT [License](LICENSE).
 
 - **Please Note:** If you choose to integrate this project into some other project using the default model or any other model trained as part of the [UVR](https://github.com/Anjok07/ultimatevocalremovergui) project, please honor the MIT license by providing credit to UVR and its developers!
 
-## Credits
+## Credits 🙏
 
 - [Anjok07](https://github.com/Anjok07) - Author of [Ultimate Vocal Remover GUI](https://github.com/Anjok07/ultimatevocalremovergui), which almost all of the code in this repo was copied from! Definitely deserving of credit for anything good from this project. Thank you!
 - [DilanBoskan](https://github.com/DilanBoskan) - Your contributions at the start of this project were essential to the success of UVR. Thank you!
 - [Kuielab & Woosung Choi](https://github.com/kuielab) - Developed the original MDX-Net AI code. 
 - [KimberleyJSN](https://github.com/KimberleyJensen) - Advised and aided the implementation of the training scripts for MDX-Net and Demucs. Thank you!
 - [Hv](https://github.com/NaJeongMo/Colab-for-MDX_B) - Helped implement chunks into the MDX-Net AI code. Thank you!
+
+## Contact 💌
+
+For questions or feedback, please raise an issue or reach out to @beveradb ([Andrew Beveridge](mailto:andrew@beveridge.uk)) directly.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `audio_separator-0.2.3/audio_separator/separator.py` & `audio_separator-0.3.1/audio_separator/separator.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,33 +1,52 @@
 import os
 import warnings
 import hashlib
 import json
-import datetime
-
+import logging
 import warnings
 import wget
 import torch
 import librosa
 import numpy as np
 import onnxruntime as ort
 import soundfile as sf
 from audio_separator.utils import spec_utils
 
 
-def print_with_timestamp(message):
-    timestamp = datetime.datetime.now().isoformat()
-    print(f"{timestamp} - {message}")
+class Separator:
+    def __init__(
+        self,
+        audio_file_path,
+        model_name="UVR_MDXNET_KARA_2",
+        model_file_dir="/tmp/audio-separator-models/",
+        output_dir=None,
+        use_cuda=False,
+        log_level=logging.DEBUG,
+        log_formatter=None,
+    ):
+        self.logger = logging.getLogger(__name__)
+        self.logger.setLevel(log_level)
+
+        log_handler = logging.StreamHandler()
+
+        if log_formatter is None:
+            log_formatter = logging.Formatter("%(asctime)s - %(levelname)s - %(module)s - %(message)s")
 
+        log_handler.setFormatter(log_formatter)
+        self.logger.addHandler(log_handler)
+
+        self.logger.debug(
+            f"Separator instantiating with input file: {audio_file_path}, model_name: {model_name}, output_dir: {output_dir}, use_cuda: {use_cuda}"
+        )
 
-class Separator:
-    def __init__(self, audio_file_path, model_name="UVR_MDXNET_KARA_2", model_file_dir="/tmp/audio-separator-models/", output_dir=None):
         self.model_name = model_name
         self.model_file_dir = model_file_dir
         self.output_dir = output_dir
+        self.use_cuda = use_cuda
 
         # Create the model directory if it does not exist
         os.makedirs(self.model_file_dir, exist_ok=True)
 
         self.audio_file_path = audio_file_path
         self.audio_file_base = os.path.splitext(os.path.basename(audio_file_path))[0]
 
@@ -46,77 +65,86 @@
         self.hop = 1024
 
         self.primary_source = None
         self.secondary_source = None
 
         warnings.filterwarnings("ignore")
         self.cpu = torch.device("cpu")
-        self.device = torch.device("cpu")
-        self.run_type = ["CPUExecutionProvider"]
+
+        if self.use_cuda:
+            self.logger.debug("Running in GPU mode")
+            self.device = torch.device("cuda")
+            self.run_type = ["CUDAExecutionProvider"]
+        else:
+            self.logger.debug("Running in CPU mode")
+            self.device = torch.device("cpu")
+            self.run_type = ["CPUExecutionProvider"]
 
     def get_model_hash(self, model_path):
         try:
             with open(model_path, "rb") as f:
                 f.seek(-10000 * 1024, 2)
                 return hashlib.md5(f.read()).hexdigest()
         except:
             return hashlib.md5(open(model_path, "rb").read()).hexdigest()
 
     def separate(self):
         model_path = os.path.join(self.model_file_dir, f"{self.model_name}.onnx")
         if not os.path.isfile(model_path):
-            print_with_timestamp(f"Model not found at path {model_path}, downloading...")
+            self.logger.debug(f"Model not found at path {model_path}, downloading...")
             wget.download(self.model_url, model_path)
 
-        print_with_timestamp("Reading model settings...")
+        self.logger.debug("Reading model settings...")
 
         model_hash = self.get_model_hash(model_path)
-        print_with_timestamp(f"Model {model_path} has hash {model_hash} ...")
+        self.logger.debug(f"Model {model_path} has hash {model_hash} ...")
 
         model_data_path = os.path.join(self.model_file_dir, "model_data.json")
         if not os.path.isfile(model_data_path):
-            print_with_timestamp(f"Model data not found at path {model_data_path}, downloading...")
+            self.logger.debug(f"Model data not found at path {model_data_path}, downloading...")
             wget.download(self.model_data_url, model_data_path)
 
         model_data_object = json.load(open(model_data_path))
         model_data = model_data_object[model_hash]
 
         self.compensate = model_data["compensate"]
         self.dim_f = model_data["mdx_dim_f_set"]
         self.dim_t = 2 ** model_data["mdx_dim_t_set"]
         self.n_fft = model_data["mdx_n_fft_scale_set"]
         self.primary_stem = model_data["primary_stem"]
         self.secondary_stem = "Vocals" if self.primary_stem == "Instrumental" else "Instrumental"
 
-        print_with_timestamp(
+        self.logger.debug(
             f"Set model data values: compensate = {self.compensate} primary_stem = {self.primary_stem} dim_f = {self.dim_f} dim_t = {self.dim_t} n_fft = {self.n_fft}"
         )
 
-        print_with_timestamp("Loading model...")
+        self.logger.debug("Loading model...")
         ort_ = ort.InferenceSession(model_path, providers=self.run_type)
         self.model_run = lambda spek: ort_.run(None, {"input": spek.cpu().numpy()})[0]
 
         self.initialize_model_settings()
-        print_with_timestamp("Running inference...")
+        self.logger.info("Running inference...")
         mdx_net_cut = True
         mix, raw_mix, samplerate = prepare_mix(self.audio_file_path, self.chunks, self.margin, mdx_net_cut=mdx_net_cut)
-        print_with_timestamp("Demixing...")
+        self.logger.info("Demixing...")
         source = self.demix_base(mix)[0]
 
-        print_with_timestamp(f"Saving {self.primary_stem} stem...")
+        self.logger.info(f"Saving {self.primary_stem} stem...")
         primary_stem_path = os.path.join(f"{self.audio_file_base}_({self.primary_stem})_{self.model_name}.wav")
         if not isinstance(self.primary_source, np.ndarray):
-            self.primary_source = spec_utils.normalize(source, self.is_normalization).T
+            self.primary_source = spec_utils.normalize(self.logger, source, self.is_normalization).T
         self.write_audio(primary_stem_path, self.primary_source, samplerate)
 
-        print_with_timestamp(f"Saving {self.secondary_stem} stem...")
+        self.logger.info(f"Saving {self.secondary_stem} stem...")
         secondary_stem_path = os.path.join(f"{self.audio_file_base}_({self.secondary_stem})_{self.model_name}.wav")
         if not isinstance(self.secondary_source, np.ndarray):
             raw_mix = self.demix_base(raw_mix, is_match_mix=True)[0] if mdx_net_cut else raw_mix
-            self.secondary_source, raw_mix = spec_utils.normalize_two_stem(source * self.compensate, raw_mix, self.is_normalization)
+            self.secondary_source, raw_mix = spec_utils.normalize_two_stem(
+                self.logger, source * self.compensate, raw_mix, self.is_normalization
+            )
             self.secondary_source = -self.secondary_source.T + raw_mix.T
         self.write_audio(secondary_stem_path, self.secondary_source, samplerate)
 
         torch.cuda.empty_cache()
         return primary_stem_path, secondary_stem_path
 
     def write_audio(self, stem_path, stem_source, samplerate):
```

### Comparing `audio_separator-0.2.3/audio_separator/utils/spec_utils.py` & `audio_separator-0.3.1/audio_separator/utils/spec_utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,42 +1,31 @@
 import librosa
 import numpy as np
 import soundfile as sf
 import math
 import random
 import math
 import platform
-import traceback
-import datetime
+import logging
 
 OPERATING_SYSTEM = platform.system()
 SYSTEM_ARCH = platform.platform()
 SYSTEM_PROC = platform.processor()
 ARM = "arm"
 
-if OPERATING_SYSTEM == "Windows":
-    from pyrubberband import pyrb
-else:
-    from audio_separator.utils import pyrb
-
 if OPERATING_SYSTEM == "Darwin":
     wav_resolution = "polyphase" if SYSTEM_PROC == ARM or ARM in SYSTEM_ARCH else "sinc_fastest"
 else:
     wav_resolution = "sinc_fastest"
 
 MAX_SPEC = "Max Spec"
 MIN_SPEC = "Min Spec"
 AVERAGE = "Average"
 
 
-def print_with_timestamp(message):
-    timestamp = datetime.datetime.now().isoformat()
-    print(f"{timestamp} - {message}")
-
-
 def crop_center(h1, h2):
     h1_shape = h1.size()
     h2_shape = h2.size()
 
     if h1_shape[3] == h2_shape[3]:
         return h1
     elif h1_shape[3] < h2_shape[3]:
@@ -114,50 +103,50 @@
     thread.join()
 
     spec = np.asfortranarray([spec_left, spec_right])
 
     return spec
 
 
-def normalize(wave, is_normalize=False):
+def normalize(logger: logging.Logger, wave, is_normalize=False):
     """Save output music files"""
     maxv = np.abs(wave).max()
     if maxv > 1.0:
-        print_with_timestamp(f"Normalization Set {is_normalize}: Input above threshold for clipping. Max:{maxv}")
+        logger.debug(f"Normalization Set {is_normalize}: Input above threshold for clipping. Max:{maxv}")
         if is_normalize:
-            print(f"The result was normalized.")
+            logger.debug(f"The result was normalized.")
             wave /= maxv
         else:
-            print(f"The result was not normalized.")
+            logger.debug(f"The result was not normalized.")
     else:
-        print_with_timestamp(f"Normalization Set {is_normalize}: Input not above threshold for clipping. Max:{maxv}")
+        logger.debug(f"Normalization Set {is_normalize}: Input not above threshold for clipping. Max:{maxv}")
 
     return wave
 
 
-def normalize_two_stem(wave, mix, is_normalize=False):
+def normalize_two_stem(logger: logging.Logger, wave, mix, is_normalize=False):
     """Save output music files"""
 
     maxv = np.abs(wave).max()
     max_mix = np.abs(mix).max()
 
     if maxv > 1.0:
-        print_with_timestamp(f"Normalization Set {is_normalize}: Primary source above threshold for clipping. Max:{maxv}")
-        print_with_timestamp(f"Normalization Set {is_normalize}: Mixture above threshold for clipping. Max:{max_mix}")
+        logger.debug(f"Normalization Set {is_normalize}: Primary source above threshold for clipping. Max:{maxv}")
+        logger.debug(f"Normalization Set {is_normalize}: Mixture above threshold for clipping. Max:{max_mix}")
         if is_normalize:
-            print(f"The result was normalized.")
+            logger.debug(f"The result was normalized.")
             wave /= maxv
             mix /= maxv
         else:
-            print(f"The result was not normalized.")
+            logger.debug(f"The result was not normalized.")
     else:
-        print_with_timestamp(f"Normalization Set {is_normalize}: Input not above threshold for clipping. Max:{maxv}")
+        logger.debug(f"Normalization Set {is_normalize}: Input not above threshold for clipping. Max:{maxv}")
 
-    print_with_timestamp(f"Normalization Set {is_normalize}: Primary source - Max:{np.abs(wave).max()}")
-    print_with_timestamp(f"Normalization Set {is_normalize}: Mixture - Max:{np.abs(mix).max()}")
+    logger.debug(f"Normalization Set {is_normalize}: Primary source - Max:{np.abs(wave).max()}")
+    logger.debug(f"Normalization Set {is_normalize}: Mixture - Max:{np.abs(mix).max()}")
 
     return wave, mix
 
 
 def combine_spectrograms(specs, mp):
     l = min([specs[i].shape[2] for i in specs])
     spec_c = np.zeros(shape=(2, mp.param["bins"] + 1, l), dtype=np.complex64)
@@ -217,60 +206,14 @@
 
     v_mask = v_mag_tmp > y_mag_tmp
     y_mag = np.clip(y_mag_tmp - v_mag_tmp * v_mask * softmask, 0, np.inf)
 
     return y_mag * np.exp(1.0j * np.angle(y))
 
 
-def merge_artifacts(y_mask, thres=0.01, min_range=64, fade_size=32):
-    mask = y_mask
-
-    try:
-        if min_range < fade_size * 2:
-            raise ValueError("min_range must be >= fade_size * 2")
-
-        idx = np.where(y_mask.min(axis=(0, 1)) > thres)[0]
-        start_idx = np.insert(idx[np.where(np.diff(idx) != 1)[0] + 1], 0, idx[0])
-        end_idx = np.append(idx[np.where(np.diff(idx) != 1)[0]], idx[-1])
-        artifact_idx = np.where(end_idx - start_idx > min_range)[0]
-        weight = np.zeros_like(y_mask)
-        if len(artifact_idx) > 0:
-            start_idx = start_idx[artifact_idx]
-            end_idx = end_idx[artifact_idx]
-            old_e = None
-            for s, e in zip(start_idx, end_idx):
-                if old_e is not None and s - old_e < fade_size:
-                    s = old_e - fade_size * 2
-
-                if s != 0:
-                    weight[:, :, s : s + fade_size] = np.linspace(0, 1, fade_size)
-                else:
-                    s -= fade_size
-
-                if e != y_mask.shape[2]:
-                    weight[:, :, e - fade_size : e] = np.linspace(1, 0, fade_size)
-                else:
-                    e += fade_size
-
-                weight[:, :, s + fade_size : e - fade_size] = 1
-                old_e = e
-
-        v_mask = 1 - y_mask
-        y_mask += weight * v_mask
-
-        mask = y_mask
-    except Exception as e:
-        error_name = f"{type(e).__name__}"
-        traceback_text = "".join(traceback.format_tb(e.__traceback__))
-        message = f'{error_name}: "{e}"\n{traceback_text}"'
-        print("Post Process Failed: ", message)
-
-    return mask
-
-
 def align_wave_head_and_tail(a, b):
     l = min([a[0].size, b[0].size])
 
     return a[:l, :l], b[:l, :l]
 
 
 def spectrogram_to_wave(spec, hop_length, mid_side, mid_side_b2, reverse, clamp=False):
@@ -564,38 +507,14 @@
         pad_value = target_dim - x_dim
         pad_tuple = (0, pad_value)
         padding_list.append(pad_tuple)
 
     return np.pad(x, tuple(padding_list), mode="constant")
 
 
-def augment_audio(export_path, audio_file, rate, is_normalization, wav_type_set, save_format=None, is_pitch=False):
-    wav, sr = librosa.load(audio_file, sr=44100, mono=False)
-
-    if wav.ndim == 1:
-        wav = np.asfortranarray([wav, wav])
-
-    if is_pitch:
-        wav_1 = pyrb.pitch_shift(wav[0], sr, rate, rbargs=None)
-        wav_2 = pyrb.pitch_shift(wav[1], sr, rate, rbargs=None)
-    else:
-        wav_1 = pyrb.time_stretch(wav[0], sr, rate, rbargs=None)
-        wav_2 = pyrb.time_stretch(wav[1], sr, rate, rbargs=None)
-
-    if wav_1.shape > wav_2.shape:
-        wav_2 = to_shape(wav_2, wav_1.shape)
-    if wav_1.shape < wav_2.shape:
-        wav_1 = to_shape(wav_1, wav_2.shape)
-
-    wav_mix = np.asfortranarray([wav_1, wav_2])
-
-    sf.write(export_path, normalize(wav_mix.T, is_normalization), sr, subtype=wav_type_set)
-    save_format(export_path)
-
-
 def average_audio(audio):
     waves = []
     wave_shapes = []
     final_waves = []
 
     for i in range(len(audio)):
         wave = librosa.load(audio[i], sr=44100, mono=False)
```

### Comparing `audio_separator-0.2.3/pyproject.toml` & `audio_separator-0.3.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "audio-separator"
-version = "0.2.3"
+version = "0.3.1"
 description = "Easy to use vocal separation on CLI or as a python package, using the amazing MDX-Net models from UVR trained by @Anjok07"
 authors = ["Andrew Beveridge <andrew@beveridge.uk>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "audio_separator"}]
 
 [tool.poetry.dependencies]
```

### Comparing `audio_separator-0.2.3/PKG-INFO` & `audio_separator-0.3.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audio-separator
-Version: 0.2.3
+Version: 0.3.1
 Summary: Easy to use vocal separation on CLI or as a python package, using the amazing MDX-Net models from UVR trained by @Anjok07
 License: MIT
 Author: Andrew Beveridge
 Author-email: andrew@beveridge.uk
 Requires-Python: >=3.9,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -16,15 +16,15 @@
 Requires-Dist: onnxruntime (>=1.13,<2.0)
 Requires-Dist: six (>=1.16,<2.0)
 Requires-Dist: soundfile (>=0.11,<0.12)
 Requires-Dist: torch (>=1.13,<2.0)
 Requires-Dist: wget (>=3,<4)
 Description-Content-Type: text/markdown
 
-# Audio Separator
+# Audio Separator 🎶
 
 [![PyPI version](https://badge.fury.io/py/audio-separator.svg)](https://badge.fury.io/py/audio-separator)
 
 Summary: Easy to use vocal separation on CLI or as a python package, using the amazing MDX-Net models from UVR trained by @Anjok07
 
 Audio Separator is a Python package that allows you to separate an audio file into two stems, primary and secondary, using a model in the ONNX format trained by @Anjok07 for use with UVR (https://github.com/Anjok07/ultimatevocalremovergui).
 
@@ -34,22 +34,22 @@
 
 - Separate audio into instrumental and vocal stems.
 - Supports all common audio formats (WAV, MP3, FLAC, M4A, etc.)
 - Ability to specify a pre-trained deep learning model in ONNX format.
 - CLI support for easy use in scripts and batch processing.
 - Python API for integration into other projects.
 
-## Installation
+## Installation 🛠️
 
 You can install Audio Separator using pip:
 
 `pip install audio-separator`
 
 
-## Usage
+## Usage 🚀
 
 ### Command Line Interface (CLI)
 
 You can use Audio Separator via the command line:
 
 ```sh
 audio-separator [audio_file] --model_name [model_name]
@@ -88,15 +88,15 @@
 ## Parameters for the Separator class
 
 - audio_file: The path to the audio file to be separated. Supports all common formats (WAV, MP3, FLAC, M4A, etc.)
 - model_name: (Optional) The name of the model to use for separation. Defaults to 'UVR_MDXNET_KARA_2', a very powerful model for Karaoke instrumental tracks.
 - model_file_dir: (Optional) Directory to cache model files in. Default: /tmp/audio-separator-models/
 - output_dir: (Optional) Directory where the separated files will be saved. If not specified, outputs to current dir.
 
-## Requirements
+## Requirements 📋
 
 Python <= 3.10 (one of the dependencies doesn't like 3.11 yet)
 
 Libraries: onnx, onnxruntime, numpy, soundfile, librosa, torch, wget, six
 
 ## Developing Locally
 
@@ -156,29 +156,33 @@
 
 ```
 poetry build
 ```
 
 This will generate the distribution packages in the dist directory - but for now only @beveradb will be able to publish to PyPI.
 
-## Contributing
+## Contributing 🤝
 
 Contributions are very much welcome! Please fork the repository and submit a pull request with your changes, and I'll try to review, merge and publish promptly!
 
 - This project is 100% open-source and free for anyone to use and modify as they wish. 
 - If the maintenance workload for this repo somehow becomes too much for me I'll ask for volunteers to share maintainership of the repo, though I don't think that is very likely
 - Development and support for the MDX-Net separation models is part of the main [UVR project](https://github.com/Anjok07/ultimatevocalremovergui), this repo is just a CLI/Python package wrapper to simplify running those models programmatically. So, if you want to try and improve the actual models, please get involved in the UVR project and look for guidance there!
 
-## License
+## License 📄
 
 This project is licensed under the MIT [License](LICENSE).
 
 - **Please Note:** If you choose to integrate this project into some other project using the default model or any other model trained as part of the [UVR](https://github.com/Anjok07/ultimatevocalremovergui) project, please honor the MIT license by providing credit to UVR and its developers!
 
-## Credits
+## Credits 🙏
 
 - [Anjok07](https://github.com/Anjok07) - Author of [Ultimate Vocal Remover GUI](https://github.com/Anjok07/ultimatevocalremovergui), which almost all of the code in this repo was copied from! Definitely deserving of credit for anything good from this project. Thank you!
 - [DilanBoskan](https://github.com/DilanBoskan) - Your contributions at the start of this project were essential to the success of UVR. Thank you!
 - [Kuielab & Woosung Choi](https://github.com/kuielab) - Developed the original MDX-Net AI code. 
 - [KimberleyJSN](https://github.com/KimberleyJensen) - Advised and aided the implementation of the training scripts for MDX-Net and Demucs. Thank you!
 - [Hv](https://github.com/NaJeongMo/Colab-for-MDX_B) - Helped implement chunks into the MDX-Net AI code. Thank you!
 
+## Contact 💌
+
+For questions or feedback, please raise an issue or reach out to @beveradb ([Andrew Beveridge](mailto:andrew@beveridge.uk)) directly.
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

