# Comparing `tmp/openlrc-0.1.4.tar.gz` & `tmp/openlrc-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openlrc-0.1.4.tar", max compression
+gzip compressed data, was "openlrc-0.1.5.tar", max compression
```

## Comparing `openlrc-0.1.4.tar` & `openlrc-0.1.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1083 2023-05-10 10:20:06.659160 openlrc-0.1.4/LICENSE
--rw-r--r--   0        0        0      106 2023-06-09 13:01:57.605311 openlrc-0.1.4/openlrc/__init__.py
--rw-r--r--   0        0        0     6642 2023-07-01 13:36:53.572387 openlrc-0.1.4/openlrc/chatbot.py
--rw-r--r--   0        0        0     2704 2023-06-27 13:49:50.307093 openlrc-0.1.4/openlrc/context.py
--rw-r--r--   0        0        0      966 2023-07-05 20:31:15.832362 openlrc-0.1.4/openlrc/exceptions.py
--rw-r--r--   0        0        0      597 2023-06-15 20:08:22.292558 openlrc-0.1.4/openlrc/logger.py
--rw-r--r--   0        0        0    13866 2023-07-06 14:20:07.448891 openlrc-0.1.4/openlrc/openlrc.py
--rw-r--r--   0        0        0     5204 2023-07-03 18:14:57.916841 openlrc-0.1.4/openlrc/opt.py
--rw-r--r--   0        0        0     7664 2023-06-27 08:09:12.518292 openlrc-0.1.4/openlrc/prompter.py
--rw-r--r--   0        0        0     6372 2023-06-29 05:51:12.383562 openlrc-0.1.4/openlrc/subtitle.py
--rw-r--r--   0        0        0    15382 2023-07-06 13:45:34.304340 openlrc-0.1.4/openlrc/transcribe.py
--rw-r--r--   0        0        0     5726 2023-06-27 18:43:39.771392 openlrc-0.1.4/openlrc/translate.py
--rw-r--r--   0        0        0     6552 2023-07-06 13:45:34.300323 openlrc-0.1.4/openlrc/utils.py
--rw-r--r--   0        0        0     1718 2023-07-06 14:29:59.404295 openlrc-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     5508 2023-07-06 14:34:39.772560 openlrc-0.1.4/README.md
--rw-r--r--   0        0        0     6960 1970-01-01 00:00:00.000000 openlrc-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1083 2023-05-10 10:20:06.659160 openlrc-0.1.5/LICENSE
+-rw-r--r--   0        0        0      106 2023-06-09 13:01:57.605311 openlrc-0.1.5/openlrc/__init__.py
+-rw-r--r--   0        0        0     6642 2023-07-01 13:36:53.572387 openlrc-0.1.5/openlrc/chatbot.py
+-rw-r--r--   0        0        0     2704 2023-06-27 13:49:50.307093 openlrc-0.1.5/openlrc/context.py
+-rw-r--r--   0        0        0      966 2023-07-05 20:31:15.832362 openlrc-0.1.5/openlrc/exceptions.py
+-rw-r--r--   0        0        0      597 2023-06-15 20:08:22.292558 openlrc-0.1.5/openlrc/logger.py
+-rw-r--r--   0        0        0    13967 2023-07-06 16:13:15.634083 openlrc-0.1.5/openlrc/openlrc.py
+-rw-r--r--   0        0        0     5204 2023-07-03 18:14:57.916841 openlrc-0.1.5/openlrc/opt.py
+-rw-r--r--   0        0        0     7664 2023-06-27 08:09:12.518292 openlrc-0.1.5/openlrc/prompter.py
+-rw-r--r--   0        0        0     6372 2023-06-29 05:51:12.383562 openlrc-0.1.5/openlrc/subtitle.py
+-rw-r--r--   0        0        0    15382 2023-07-06 13:45:34.304340 openlrc-0.1.5/openlrc/transcribe.py
+-rw-r--r--   0        0        0     5726 2023-06-27 18:43:39.771392 openlrc-0.1.5/openlrc/translate.py
+-rw-r--r--   0        0        0     6552 2023-07-06 13:45:34.300323 openlrc-0.1.5/openlrc/utils.py
+-rw-r--r--   0        0        0     1718 2023-07-07 02:24:49.837818 openlrc-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     5606 2023-07-06 14:38:43.653605 openlrc-0.1.5/README.md
+-rw-r--r--   0        0        0     7055 1970-01-01 00:00:00.000000 openlrc-0.1.5/PKG-INFO
```

### Comparing `openlrc-0.1.4/LICENSE` & `openlrc-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `openlrc-0.1.4/openlrc/chatbot.py` & `openlrc-0.1.5/openlrc/chatbot.py`

 * *Files identical despite different names*

### Comparing `openlrc-0.1.4/openlrc/context.py` & `openlrc-0.1.5/openlrc/context.py`

 * *Files identical despite different names*

### Comparing `openlrc-0.1.4/openlrc/exceptions.py` & `openlrc-0.1.5/openlrc/exceptions.py`

 * *Files identical despite different names*

### Comparing `openlrc-0.1.4/openlrc/logger.py` & `openlrc-0.1.5/openlrc/logger.py`

 * *Files identical despite different names*

### Comparing `openlrc-0.1.4/openlrc/openlrc.py` & `openlrc-0.1.5/openlrc/openlrc.py`

 * *Files 0% similar despite different names*

```diff
@@ -137,31 +137,33 @@
             logger.info(f'Got transcription: {transcribed_path}')
             transcribed_sub = Subtitle.from_json(transcribed_path)
             transcribed_opt_sub = self.post_process(transcribed_sub, update_name=True)
             audio_name = transcribed_path.stem.replace('_transcribed', '')
 
             # xxx_transcribed_optimized_translated.json
             translated_path = extend_filename(transcribed_opt_sub.filename, '_translated')
-            if skip_trans:
-                final_subtitle = transcribed_opt_sub
-            else:
+
+            final_subtitle = transcribed_opt_sub
+            if not skip_trans:
                 with Timer('Translation process'):
                     try:
                         final_subtitle = self._translate(audio_name, prompter, target_lang, transcribed_opt_sub,
                                                          translated_path)
                     except Exception as e:
                         self.exception = e
 
+            final_subtitle.filename = Path(translated_path.parent / f'{audio_name}.json')
+
             final_subtitle.to_lrc()
             if audio_name in self.from_video:
                 final_subtitle.to_srt()
             logger.info(f'Translation fee til now: {self.api_fee:.4f} USD')
 
     def _translate(self, audio_name, prompter, target_lang, transcribed_opt_sub, translated_path):
-        json_filename = Path(audio_name).with_suffix('.json')
+        json_filename = Path(translated_path.parent / audio_name).with_suffix('.json')
         compare_path = Path(translated_path.parent, f'{audio_name}_compare.json')
         if not translated_path.exists():
             if not compare_path.exists():
                 # Translate the transcribed json
                 translator = GPTTranslator(prompter=prompter, fee_limit=self.fee_limit)
                 context = self.context
```

### Comparing `openlrc-0.1.4/openlrc/opt.py` & `openlrc-0.1.5/openlrc/opt.py`

 * *Files identical despite different names*

### Comparing `openlrc-0.1.4/openlrc/prompter.py` & `openlrc-0.1.5/openlrc/prompter.py`

 * *Files identical despite different names*

### Comparing `openlrc-0.1.4/openlrc/subtitle.py` & `openlrc-0.1.5/openlrc/subtitle.py`

 * *Files identical despite different names*

### Comparing `openlrc-0.1.4/openlrc/transcribe.py` & `openlrc-0.1.5/openlrc/transcribe.py`

 * *Files identical despite different names*

### Comparing `openlrc-0.1.4/openlrc/translate.py` & `openlrc-0.1.5/openlrc/translate.py`

 * *Files identical despite different names*

### Comparing `openlrc-0.1.4/openlrc/utils.py` & `openlrc-0.1.5/openlrc/utils.py`

 * *Files identical despite different names*

### Comparing `openlrc-0.1.4/pyproject.toml` & `openlrc-0.1.5/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [virtualenvs]
 create = true
 in-project = true
 
 [tool.poetry]
 name = "openlrc"
-version = "0.1.4"
+version = "0.1.5"
 description = "Transcribe (whisper) and translate (gpt) voice into LRC file."
 license = "MIT"
 authors = [
     "Hao Zheng <zhenghaosustc@gmail.com>"
 ]
 readme = "README.md"
 homepage = "https://github.com/zh-plus/Open-Lyrics"
```

### Comparing `openlrc-0.1.4/README.md` & `openlrc-0.1.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -62,14 +62,17 @@
 
 # Path can contain video
 lrcer.run(['./data/test_audio.mp3', './data/test_video.mp4'], target_lang='zh-cn')
 # Generate translated ./data/test_audio.lrc and ./data/test_video.srt
 
 # Use context.yaml to improve translation
 lrcer.run('./data/test.mp3', target_lang='zh-cn', context_path='./data/context.yaml')
+
+# To skip translation process
+lrcer.run('./data/test.mp3', target_lang='en', skip_trans=True)
 ```
 
 ### Context
 
 Utilize the available context to enhance the quality of your translation.
 Save them as `context.yaml` in the same directory as your audio file.
```

### Comparing `openlrc-0.1.4/PKG-INFO` & `openlrc-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openlrc
-Version: 0.1.4
+Version: 0.1.5
 Summary: Transcribe (whisper) and translate (gpt) voice into LRC file.
 Home-page: https://github.com/zh-plus/Open-Lyrics
 License: MIT
 Keywords: openai-gpt3,whisper,voice transcribe,lrc
 Author: Hao Zheng
 Author-email: zhenghaosustc@gmail.com
 Requires-Python: >=3.8,<4.0
@@ -101,14 +101,17 @@
 
 # Path can contain video
 lrcer.run(['./data/test_audio.mp3', './data/test_video.mp4'], target_lang='zh-cn')
 # Generate translated ./data/test_audio.lrc and ./data/test_video.srt
 
 # Use context.yaml to improve translation
 lrcer.run('./data/test.mp3', target_lang='zh-cn', context_path='./data/context.yaml')
+
+# To skip translation process
+lrcer.run('./data/test.mp3', target_lang='en', skip_trans=True)
 ```
 
 ### Context
 
 Utilize the available context to enhance the quality of your translation.
 Save them as `context.yaml` in the same directory as your audio file.
```

