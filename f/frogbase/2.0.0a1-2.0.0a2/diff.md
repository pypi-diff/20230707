# Comparing `tmp/frogbase-2.0.0a1.tar.gz` & `tmp/frogbase-2.0.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frogbase-2.0.0a1.tar", max compression
+gzip compressed data, was "frogbase-2.0.0a2.tar", max compression
```

## Comparing `frogbase-2.0.0a1.tar` & `frogbase-2.0.0a2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1070 2023-06-17 23:46:09.847926 frogbase-2.0.0a1/LICENSE
--rw-r--r--   0        0        0     3836 2023-07-05 09:17:15.496901 frogbase-2.0.0a1/README.md
--rw-r--r--   0        0        0       27 2023-07-03 04:12:13.959861 frogbase-2.0.0a1/frogbase/__init__.py
--rw-r--r--   0        0        0      984 2023-07-03 07:18:00.093889 frogbase-2.0.0a1/frogbase/__main__.py
--rw-r--r--   0        0        0     7182 2023-07-05 00:48:25.059735 frogbase-2.0.0a1/frogbase/captions.py
--rw-r--r--   0        0        0      946 2023-07-05 07:49:31.064883 frogbase-2.0.0a1/frogbase/config.py
--rw-r--r--   0        0        0    15740 2023-07-05 08:32:20.537021 frogbase-2.0.0a1/frogbase/core.py
--rw-r--r--   0        0        0    29544 2023-07-05 00:48:25.423726 frogbase-2.0.0a1/frogbase/media.py
--rw-r--r--   0        0        0    25385 2023-07-05 08:32:57.776032 frogbase-2.0.0a1/frogbase/models.py
--rw-r--r--   0        0        0     2975 2023-07-05 09:18:04.319830 frogbase-2.0.0a1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-01 20:27:47.202722 frogbase-2.0.0a1/tests/__init__.py
--rw-r--r--   0        0        0      242 2023-07-04 02:06:26.660985 frogbase-2.0.0a1/tests/conftest.py
--rw-r--r--   0        0        0     1160 2023-07-05 00:47:50.368601 frogbase-2.0.0a1/tests/test_config.py
--rw-r--r--   0        0        0     6031 2023-07-05 00:48:25.835716 frogbase-2.0.0a1/tests/test_core.py
--rw-r--r--   0        0        0     3289 2023-07-05 00:48:24.683744 frogbase-2.0.0a1/tests/test_media.py
--rw-r--r--   0        0        0     5361 1970-01-01 00:00:00.000000 frogbase-2.0.0a1/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-06-17 23:46:09.847926 frogbase-2.0.0a2/LICENSE
+-rw-r--r--   0        0        0     4016 2023-07-06 21:02:27.903992 frogbase-2.0.0a2/README.md
+-rw-r--r--   0        0        0       27 2023-07-05 10:01:59.615234 frogbase-2.0.0a2/frogbase/__init__.py
+-rw-r--r--   0        0        0      984 2023-07-05 10:01:59.615234 frogbase-2.0.0a2/frogbase/__main__.py
+-rw-r--r--   0        0        0     8263 2023-07-06 22:12:19.492087 frogbase-2.0.0a2/frogbase/captions.py
+-rw-r--r--   0        0        0      946 2023-07-05 10:01:59.615234 frogbase-2.0.0a2/frogbase/config.py
+-rw-r--r--   0        0        0    16491 2023-07-06 23:28:55.421394 frogbase-2.0.0a2/frogbase/core.py
+-rw-r--r--   0        0        0    29577 2023-07-06 21:59:29.299325 frogbase-2.0.0a2/frogbase/media.py
+-rw-r--r--   0        0        0    25161 2023-07-06 22:11:30.461311 frogbase-2.0.0a2/frogbase/models.py
+-rw-r--r--   0        0        0     2975 2023-07-06 23:33:01.546938 frogbase-2.0.0a2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-05 10:01:59.619233 frogbase-2.0.0a2/tests/__init__.py
+-rw-r--r--   0        0        0      242 2023-07-05 10:01:59.619233 frogbase-2.0.0a2/tests/conftest.py
+-rw-r--r--   0        0        0     1160 2023-07-05 10:01:59.619233 frogbase-2.0.0a2/tests/test_config.py
+-rw-r--r--   0        0        0     6031 2023-07-05 10:01:59.619233 frogbase-2.0.0a2/tests/test_core.py
+-rw-r--r--   0        0        0     3289 2023-07-05 10:01:59.619233 frogbase-2.0.0a2/tests/test_media.py
+-rw-r--r--   0        0        0     5541 1970-01-01 00:00:00.000000 frogbase-2.0.0a2/PKG-INFO
```

### Comparing `frogbase-2.0.0a1/LICENSE` & `frogbase-2.0.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `frogbase-2.0.0a1/README.md` & `frogbase-2.0.0a2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,23 @@
 **FrogBase** (previously whisper-ui) simplifies the `download-transcribe-embed-index` workflow for multi-media content.
 It does so by linking content from various platforms
 ([yt_dlp](https://github.com/yt-dlp/yt-dlp))
 with speech-to-text models ([OpenAI's Whisper](https://github.com/openai/whisper)),
 image & text encoders ([SentenceTransformers](https://github.com/UKPLab/sentence-transformers)),
 and embedding stores ([hnswlib](https://github.com/nmslib/hnswlib)).
 
+```python
+from frogbase import FrogBase
+fb = FrogBase()
+fb.demo()
+fb.search("What is the name of the squeaky frog?")
+```
+
+> [Full Documentation](https://hayabhay.github.io/frogbase/) (WIP).
+
 _FrogBase also comes with a **ready-to-use UI for non-technical users!**_
 
 https://user-images.githubusercontent.com/6735526/216852681-53b6c3db-3e74-4c86-806f-6f6774a9003a.mp4
 
 [![PyPI](https://img.shields.io/pypi/v/frogbase.svg)][pypi_]
 [![Status](https://img.shields.io/pypi/status/frogbase.svg)][status]
 [![Python Version](https://img.shields.io/pypi/pyversions/frogbase)][python version]
@@ -75,34 +84,32 @@
 ### Non-technical Users
 
 This section is for non-technical users who want to use FrogBase primarily through the accompanying Streamlit UI.
 
 1. Download the latest release of FrogBase from [here](https://github.com/hayabhay/frogbase/archive/refs/heads/main.zip) and unzip it.
    Or, you can also clone the repository
    `console
-   git clone https://github.com/hayabhay/frogbase.git
-   `
-
+git clone https://github.com/hayabhay/frogbase.git
+`
 
 2. Install FrogBase dependencies manually and run the UI.
 
    > Note: This also requires `ffmpeg` to be installed on your system. You can install it using `sudo apt install ffmpeg` on Ubuntu.
 
    1. Using pip
 
       ```console
       pip install frogbase streamlit
       streamlit run ui/01_🏠_Home.py
       ```
 
 > [Coming soon] Instructions, environment for installation using Docker & Anaconda
-   
+
 ## Links
 
 - [Documentation](https://hayabhay.github.io/frogbase/)
 - [Issues](https://github.com/hayabhay/frogbase/issues) & [Discussions](https://github.com/hayabhay/frogbase/discussions)
 - [Discord](https://discord.gg/e23YJWqu)
 - [History](docs/history.md)
 - [Roadmap](docs/roadmap.md)
 - [Contributing Guide](docs/contributing.md)
 - [License](LICENSE) (MIT)
-
```

### Comparing `frogbase-2.0.0a1/frogbase/__main__.py` & `frogbase-2.0.0a2/frogbase/__main__.py`

 * *Files identical despite different names*

### Comparing `frogbase-2.0.0a1/frogbase/captions.py` & `frogbase-2.0.0a2/frogbase/captions.py`

 * *Files 10% similar despite different names*

```diff
@@ -84,23 +84,39 @@
         Args:
             captions: The captions object or id to load from the .vtt file.
 
         Returns:
             Dictionary containing the captions data in the form of a standard captions object.
             This is a subset of openai's transcript format.
         """
-        if fmt == "json":
-            json_fname = f"{self._loc.stem}.{fmt}"
-            with open((self._loc.parent / json_fname).resolve()) as f:
-                return json.load(f)
-        elif fmt == "vtt" or fmt == "srt":
-            return webvtt.read(str(self._loc.resolve()))
+        if fmt == "vtt" or fmt == "srt":
+            captions_reader = (
+                webvtt.read(str(self._loc.resolve())) if fmt == "vtt" else webvtt.from_srt(str(self._loc.resolve()))
+            )
+            for segment_id, captions in enumerate(captions_reader):
+                yield {
+                    "id": segment_id,
+                    "start": captions.start_in_seconds,
+                    "end": captions.end_in_seconds,
+                    "start_str": captions.start,
+                    "end_str": captions.end,
+                    "text": captions.text,
+                }
         else:
             raise ValueError(f"Unsupported or missing captions for '{fmt}' format.")
 
+    def _load_whisper_json(self) -> dict[str, Any]:
+        """Internal method to load whisper's json dump if available."""
+        json_fname = f"{self._loc.stem}.{json}"
+        if not (self._loc.parent / json_fname).exists():
+            raise ValueError(f"Missing whisper json file for {self._loc.name}")
+        else:
+            with open((self._loc.parent / json_fname).resolve()) as f:
+                return json.load(f)
+
     def delete(self, bkup_files: bool = True) -> None:
         """Delete this captions object from db and file."""
         self._table.remove(Query().id == self.id)
         self._logger.info(f"Deleted captions from db: {id}")
 
         if bkup_files:
             # Remove the captions info file from disk.
@@ -151,16 +167,24 @@
         Returns:
             A list of all captions objects.
         """
         captions_dicts = self._table.search(Query().media_id == self.media_id)
         captions_dicts = sorted(captions_dicts, key=lambda x: x["created"], reverse=True)
         return [Captions(config=self._config, **captions_dict) for captions_dict in captions_dicts]
 
-    def latest(self) -> Captions:
+    # TODO: Fix this.
+    def latest(self, prefer_subtitles=True) -> Captions:
         """Get the latest captions object from db for the given media.
 
         Returns:
             The latest captions object.
         """
         captions_dicts = self._table.search(Query().media_id == self.media_id)
         captions_dicts = sorted(captions_dicts, key=lambda x: x["created"], reverse=True)
-        return Captions(config=self._config, **captions_dicts[0]) if captions_dicts else None
+        captions_dict = None
+        if prefer_subtitles:
+            for captions_dict in captions_dicts:
+                if captions_dict["kind"] == "subtitles":
+                    break
+        # Else pick the first one if it exists.
+        captions_dict = captions_dict or captions_dicts[0]
+        return Captions(config=self._config, **captions_dict) if captions_dict else None
```

### Comparing `frogbase-2.0.0a1/frogbase/config.py` & `frogbase-2.0.0a2/frogbase/config.py`

 * *Files identical despite different names*

### Comparing `frogbase-2.0.0a1/frogbase/core.py` & `frogbase-2.0.0a2/frogbase/core.py`

 * *Files 6% similar despite different names*

```diff
@@ -104,14 +104,17 @@
         # NOTE: The library setter initializes a "session" of sorts. Specifically,
         # 1. It sets the library name & path along with creating the directory.
         # 2. It initializes tinydb & purges/clears/recover db as needed.
         # 3. It updates table references & managers for the FrogBase instance.
         # In addition, a fair number of variables are set up in the library setter.
         self.library = self._default_library
 
+        self._media_buffer = []
+        self._index = None
+
         # NOTE: Do not add any code after the library setter unless they're
         # related to the library setter.
 
     def __repr__(self) -> str:
         return f"<FrogBase: {self._libdir}>"
 
     def __str__(self) -> str:
@@ -179,15 +182,23 @@
 
         # First check if the tinydb instance exists and if it is compatible
         # with the current version of FrogBase. If not, delete the tinydb
         # json and re-create it.
         # NOTE: Right now any version change will re-create tinydb and purge
         # all existing data to ensure compatibility. Later, this can be updated
         # to only re-create the tinydb data if the minor version changes.
-        db_meta = self._db.get(Query().type == "meta") if self._db else None
+        # NOTE: Temporary hack to kill tinydb if it fails to load. Fix this later
+        try:
+            db_meta = self._db.get(Query().type == "meta") if self._db else None
+        except Exception as e:
+            self._logger.error(f"Failed to load tinydb instance. Error: {e}")
+            self._db.close()
+            self._dbpath.unlink()
+            self._db = None
+            
         if db_meta and db_meta["__version__"] < self._version:
             self._logger.info(f"Existing tinydb version: {db_meta['__version__']} is stale. Removing.")
             self._db.close()
             self._dbpath.unlink()
             self._db = None
 
         # Next, if the tinydb instance never existed or was deleted from being stale, create a new one.
@@ -290,62 +301,68 @@
 
         self.models.embed(media, embedder, model, keep_model_in_memory, overwrite, **params)
 
         return self
 
     def index(
         self,
-        media: None | Media | list[Media] = None,
+        # media: None | Media | list[Media] = None,
         indexer: str | None = None,
         embedding_source: str | None = None,
         **params: dict[str, Any],
     ) -> dict[str, Any]:
         """Builds a search index from the embedded media."""
-        # If running without arguments, assume it is running in chain mode.
-        # If nothing is in the media buffer, use all media in the library.
-        if not media:
-            if self._media_buffer:
-                self._logger.info(f"Building index for {len(self._media_buffer)} media in the batch.")
-                media = self._media_buffer
-            else:
-                self._logger.info("Building index for all the media in the library.")
-                media = self.media.all()
+        # TODO: Fix this
+        # # If running without arguments, assume it is running in chain mode.
+        # # If nothing is in the media buffer, use all media in the library.
+        # if not media:
+        #     if self._media_buffer:
+        #         self._logger.info(f"Building index for {len(self._media_buffer)} media in the batch.")
+        #         media = self._media_buffer
+        #     else:
+        #         self._logger.info("Building index for all the media in the library.")
+        #         media = self.media.all()
 
-        self._index = self.models.index(media, indexer, embedding_source, **params)
+        self._index = self.models.index(indexer, embedding_source, **params)
+        # self._index = self.models.index(media, indexer, embedding_source, **params)
 
         return self._index
 
     # NOTE: This is currently a hacky function just for the Streamlit UI
     # TODO: This needs to be cleaned up
     def search(
         self,
         query: str,
         k: int = 10,
         index: None | dict[str, Any] = None,
     ) -> list[dict[str, Any]]:
         """Searches the index for the query string."""
+        # TODO: Fix this
         if not index:
-            index = self._index
-
+            if not self._index:
+                index = self.index()
+            else:
+                index = self._index
         if not index:
             raise ValueError("No index found. Please load an index first.")
 
         # First encode the query
         query = self._index["encoder"].encode(query)
         # Then search the index
-        segment_ids, distances = self._index["index"].knn_query(query, k=k)
+        entity_ids, distances = self._index["index"].knn_query(query, k=k)
 
         results = []
-        for segment_id, distance in zip(segment_ids[0], distances[0]):
+        for entity_id, distance in zip(entity_ids[0], distances[0]):
             # Get the label for the segment
-            label = self._index["meta"][segment_id]
-            media_id, start_time = label.split("::")
-            results.append(
-                {"media": self.media.get(media_id), "start_time": float(start_time), "score": float(1 - distance)}
-            )
+            label = self._index["meta"][entity_id]
+            media_id, caption_id, segment_id, start_time = label.split("::")
+            media_obj = self.media.get(media_id)
+            captions_obj = media_obj.captions.get(caption_id)
+            captions = list(captions_obj.load())
+            results.append({"media": media_obj, "segment": captions[int(segment_id)], "score": float(1 - distance)})
 
         return results
 
     def demo(self) -> None:
         """Runs a demo version of the entire FrogBase pipeline.
         1. Downloads a youtube video.
         2. Transcribes the video using a speech-to-text model.
```

### Comparing `frogbase-2.0.0a1/frogbase/media.py` & `frogbase-2.0.0a2/frogbase/media.py`

 * *Files 0% similar despite different names*

```diff
@@ -367,15 +367,15 @@
                     # Rename captions file.
                     vtt_file.rename(newfilepath)
 
                     # Add captions to FrogBase.
                     captions_obj = Captions(
                         id=captions_id,
                         media_id=media_id,
-                        loc=str(newfilepath),
+                        loc=str(newfilepath.relative_to(self._config.libdir)),
                         infoloc=str(
                             (infojson.parent / ".bkup" / f"{captions_id}.captions.fb.json").relative_to(
                                 self._config.libdir
                             )
                         ),
                         fmt="vtt",
                         kind=kind,
```

### Comparing `frogbase-2.0.0a1/frogbase/models.py` & `frogbase-2.0.0a2/frogbase/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -395,44 +395,29 @@
             # An additional flag to overwrite embeddings is added as a stop-gap measure.
             embed_id = hashlib.sha256(f"{media_obj.id}{model_name}".encode()).hexdigest()[:16]
 
             # If the embedding already exists, skip it.
             if embed_id in embeddings and not overwrite:
                 self._logger.info(f"Embedding <id: {embed_id}> already exists. Skipping.")
                 continue
-
-            # Load caption segments
-            segments = [{"start": int(c._start), "end": int(c._end), "text": c.text} for c in captions_obj.load()]
-
-            # NOTE: Running a window over segments make the embeddings somewhat fuzzy
-            # NOTE: It is better for retrieval to start early than overshoot the end
-            # TODO: Experiment and find the best window size. For now, each segment is considered as-is
-            # segment_texts = []
-            # # For each caption segment, embed it
-            # for i in range(len(segments)):
-            #     # Get the caption text
-            #     segment_text = [segments[i]["text"]]
-            #     for j in range(i + 1, len(segments)):
-            #         segment_text += segments[j]["text"]
-            #         if segments[j]["start"] > segments[i]["start"] + 10:
-            #             break
-            #     # Combine the caption text and lookahead text
-            #     segment_texts.append({
-            #         "start": int(segments[i]["start"]),
-            #         "text": " ".join(segment_text)
-            #     })
+            # Load captions
+            # TODO: Experiment with adding windows over caption segments instead of a single segment
+            captions = list(captions_obj.load())
 
             # Embed caption segments
-            features = model.encode([s["text"] for s in segments], show_progress_bar=True, convert_to_numpy=True)
+            features = model.encode(
+                [segment["text"] for segment in captions], show_progress_bar=True, convert_to_numpy=True
+            )
             embeddings[embed_id] = {
                 "media_id": media_obj.id,
                 "captions_id": captions_obj.id,
                 "model": model_name,
                 "embeddings": features,
-                "timestamps": [s["start"] for s in segments],
+                "start_timestamps": [segment["start"] for segment in captions],
+                "segment_ids": [segment["id"] for segment in captions],
             }
 
             # Add the media object to the list of embedded media
             embedded_media.append(media_obj)
 
         # Save the embeddings to the vector cache
         with open(embeddings_cache, "wb") as f:
@@ -444,24 +429,28 @@
 
         return embedded_media
 
     # TODO: Separate indexing bit out of models to manage it separately
     # ========================== Indexing ==========================
     def index(
         self,
-        media: None | Media | list[Media] = None,
+        # media: None | Media | list[Media] = None,
         indexer: str | None = None,
         embedding_source: str | None = None,
         **params: dict[str, Any],
     ) -> dict[str, Any]:
         """Index one or more media with a specified indexing engine and parameters."""
+        # NOTE: This is a placeholder for demo & testing purposes.
+        # TODO: Add functionality to manage both indices & embeddings within them
+        # This is especially important if and when new embeddings are generated from
+        # different transcribers
 
         # If media is not a list, convert it to a list.
-        if not isinstance(media, list):
-            media = [media]
+        # if not isinstance(media, list):
+        #     media = [media]
 
         if indexer and indexer not in self._allowed_indexers:
             self._logger.error(f"Indexer {indexer} not found. Using default indexer.")
             indexer = None
 
         # Set indexer to default if not specified or invalid
         indexer = indexer if indexer else self._default_indexer
@@ -529,21 +518,29 @@
             index.init_index(
                 max_elements=max_elements, ef_construction=model_settings.ef_construction, M=model_settings.M
             )
             index_meta = {}
 
         # Add the embeddings to the index
         # Labels are media ids and start times
+        # TODO: Refactor.
         labels = []
         data = []
         indexed = set(index_meta.values())
         for meta in embeddings.values():
-            # If the first element is indexed, assume all elements are indexed
-            if f"{meta['media_id']}::{meta['timestamps'][0]}" not in indexed:
-                labels += [f"{meta['media_id']}::{st}" for st in meta["timestamps"]]
+            label_prefix = f"{meta['media_id']}::{meta['captions_id']}"
+            skipped = False
+            for segment_id, start_timestamp in zip(meta["segment_ids"], meta["start_timestamps"]):
+                label = f"{label_prefix}::{segment_id}::{start_timestamp}"
+                # If the first element is indexed, assume all elements are indexed
+                if label in indexed:
+                    skipped = True
+                    break
+                labels.append(label)
+            if not skipped:
                 data.append(meta["embeddings"])
 
         # Update label maps
         ids = []
         label_map = {}
         latest_index_value = index.element_count
         for i, label in enumerate(labels):
```

### Comparing `frogbase-2.0.0a1/pyproject.toml` & `frogbase-2.0.0a2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool]
 
 # ==== Poetry ====
 [tool.poetry]
 name = "frogbase"
-version = "2.0.0a1"
+version = "2.0.0a2"
 description = "FrogBase simplifies the download-transcribe-embed-index workflow for multi-media content. It does so by linking content from various platforms with speech-to-text models, image & text encoders and embedding stores."
 homepage = "https://hayabhay.github.io/frogbase"
 repository = "https://github.com/hayabhay/frogbase"
 documentation = "https://hayabhay.github.io/frogbase"
 authors = ["Abhay Kashyap"]
 readme = "README.md"
 license =  "MIT"
```

### Comparing `frogbase-2.0.0a1/tests/test_config.py` & `frogbase-2.0.0a2/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `frogbase-2.0.0a1/tests/test_core.py` & `frogbase-2.0.0a2/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `frogbase-2.0.0a1/tests/test_media.py` & `frogbase-2.0.0a2/tests/test_media.py`

 * *Files identical despite different names*

### Comparing `frogbase-2.0.0a1/PKG-INFO` & `frogbase-2.0.0a2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frogbase
-Version: 2.0.0a1
+Version: 2.0.0a2
 Summary: FrogBase simplifies the download-transcribe-embed-index workflow for multi-media content. It does so by linking content from various platforms with speech-to-text models, image & text encoders and embedding stores.
 Home-page: https://hayabhay.github.io/frogbase
 License: MIT
 Author: Abhay Kashyap
 Requires-Python: >=3.8, !=2.7.*, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*, !=3.6.*, !=3.7.*
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
@@ -36,14 +36,23 @@
 **FrogBase** (previously whisper-ui) simplifies the `download-transcribe-embed-index` workflow for multi-media content.
 It does so by linking content from various platforms
 ([yt_dlp](https://github.com/yt-dlp/yt-dlp))
 with speech-to-text models ([OpenAI's Whisper](https://github.com/openai/whisper)),
 image & text encoders ([SentenceTransformers](https://github.com/UKPLab/sentence-transformers)),
 and embedding stores ([hnswlib](https://github.com/nmslib/hnswlib)).
 
+```python
+from frogbase import FrogBase
+fb = FrogBase()
+fb.demo()
+fb.search("What is the name of the squeaky frog?")
+```
+
+> [Full Documentation](https://hayabhay.github.io/frogbase/) (WIP).
+
 _FrogBase also comes with a **ready-to-use UI for non-technical users!**_
 
 https://user-images.githubusercontent.com/6735526/216852681-53b6c3db-3e74-4c86-806f-6f6774a9003a.mp4
 
 [![PyPI](https://img.shields.io/pypi/v/frogbase.svg)][pypi_]
 [![Status](https://img.shields.io/pypi/status/frogbase.svg)][status]
 [![Python Version](https://img.shields.io/pypi/pyversions/frogbase)][python version]
@@ -106,35 +115,33 @@
 ### Non-technical Users
 
 This section is for non-technical users who want to use FrogBase primarily through the accompanying Streamlit UI.
 
 1. Download the latest release of FrogBase from [here](https://github.com/hayabhay/frogbase/archive/refs/heads/main.zip) and unzip it.
    Or, you can also clone the repository
    `console
-   git clone https://github.com/hayabhay/frogbase.git
-   `
-
+git clone https://github.com/hayabhay/frogbase.git
+`
 
 2. Install FrogBase dependencies manually and run the UI.
 
    > Note: This also requires `ffmpeg` to be installed on your system. You can install it using `sudo apt install ffmpeg` on Ubuntu.
 
    1. Using pip
 
       ```console
       pip install frogbase streamlit
       streamlit run ui/01_🏠_Home.py
       ```
 
 > [Coming soon] Instructions, environment for installation using Docker & Anaconda
-   
+
 ## Links
 
 - [Documentation](https://hayabhay.github.io/frogbase/)
 - [Issues](https://github.com/hayabhay/frogbase/issues) & [Discussions](https://github.com/hayabhay/frogbase/discussions)
 - [Discord](https://discord.gg/e23YJWqu)
 - [History](docs/history.md)
 - [Roadmap](docs/roadmap.md)
 - [Contributing Guide](docs/contributing.md)
 - [License](LICENSE) (MIT)
 
-
```

