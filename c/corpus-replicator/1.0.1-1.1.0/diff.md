# Comparing `tmp/corpus-replicator-1.0.1.tar.gz` & `tmp/corpus-replicator-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "corpus-replicator-1.0.1.tar", last modified: Tue Jun 27 18:31:10 2023, max compression
+gzip compressed data, was "corpus-replicator-1.1.0.tar", last modified: Fri Jul  7 15:49:36 2023, max compression
```

## Comparing `corpus-replicator-1.0.1.tar` & `corpus-replicator-1.1.0.tar`

### file list

```diff
@@ -1,61 +1,65 @@
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-27 18:31:10.485582 corpus-replicator-1.0.1/
--rw-r--r--   0 worker    (1000) worker    (1000)      440 2023-06-27 18:31:02.000000 corpus-replicator-1.0.1/.gitignore
--rw-r--r--   0 worker    (1000) worker    (1000)     2157 2023-06-27 18:31:02.000000 corpus-replicator-1.0.1/.pre-commit-config.yaml
--rw-r--r--   0 worker    (1000) worker    (1000)     3789 2023-06-27 18:31:02.000000 corpus-replicator-1.0.1/.taskcluster.yml
--rw-r--r--   0 worker    (1000) worker    (1000)      689 2023-06-27 18:31:02.000000 corpus-replicator-1.0.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 worker    (1000) worker    (1000)    15550 2023-06-27 18:31:02.000000 corpus-replicator-1.0.1/LICENSE.md
--rw-r--r--   0 worker    (1000) worker    (1000)       44 2023-06-27 18:31:02.000000 corpus-replicator-1.0.1/MANIFEST.in
--rw-r--r--   0 worker    (1000) worker    (1000)     2892 2023-06-27 18:31:10.485582 corpus-replicator-1.0.1/PKG-INFO
--rw-r--r--   0 worker    (1000) worker    (1000)     2232 2023-06-27 18:31:02.000000 corpus-replicator-1.0.1/README.md
--rw-r--r--   0 worker    (1000) worker    (1000)      864 2023-06-27 18:31:02.000000 corpus-replicator-1.0.1/pyproject.toml
--rw-r--r--   0 worker    (1000) worker    (1000)      976 2023-06-27 18:31:10.485582 corpus-replicator-1.0.1/setup.cfg
--rwxr-xr-x   0 worker    (1000) worker    (1000)      370 2023-06-27 18:31:02.000000 corpus-replicator-1.0.1/setup.py
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-27 18:31:10.473582 corpus-replicator-1.0.1/src/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-27 18:31:10.477582 corpus-replicator-1.0.1/src/corpus_replicator/
--rw-r--r--   0 worker    (1000) worker    (1000)        0 2023-06-27 18:31:02.000000 corpus-replicator-1.0.1/src/corpus_replicator/__init__.py
--rw-r--r--   0 worker    (1000) worker    (1000)      230 2023-06-27 18:31:02.000000 corpus-replicator-1.0.1/src/corpus_replicator/__main__.py
--rw-r--r--   0 worker    (1000) worker    (1000)     8344 2023-06-27 18:31:02.000000 corpus-replicator-1.0.1/src/corpus_replicator/common.py
--rw-r--r--   0 worker    (1000) worker    (1000)    10466 2023-06-27 18:31:02.000000 corpus-replicator-1.0.1/src/corpus_replicator/core.py
--rw-r--r--   0 worker    (1000) worker    (1000)     2758 2023-06-27 18:31:02.000000 corpus-replicator-1.0.1/src/corpus_replicator/generate_corpus.py
--rw-r--r--   0 worker    (1000) worker    (1000)     6350 2023-06-27 18:31:02.000000 corpus-replicator-1.0.1/src/corpus_replicator/generate_template.py
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-27 18:31:10.485582 corpus-replicator-1.0.1/src/corpus_replicator/recipes/
--rw-r--r--   0 worker    (1000) worker    (1000)      251 2023-06-27 18:31:02.000000 corpus-replicator-1.0.1/src/corpus_replicator/recipes/animation_apng_png_ffmpeg.yml
--rw-r--r--   0 worker    (1000) worker    (1000)      216 2023-06-27 18:31:02.000000 corpus-replicator-1.0.1/src/corpus_replicator/recipes/animation_gif_gif_ffmpeg.yml
--rw-r--r--   0 worker    (1000) worker    (1000)      217 2023-06-27 18:31:02.000000 corpus-replicator-1.0.1/src/corpus_replicator/recipes/animation_webp_webp_libwebp.yml
--rw-r--r--   0 worker    (1000) worker    (1000)      293 2023-06-27 18:31:02.000000 corpus-replicator-1.0.1/src/corpus_replicator/recipes/audio_aac_mp4_ffmpeg.yml
--rw-r--r--   0 worker    (1000) worker    (1000)      659 2023-06-27 18:31:02.000000 corpus-replicator-1.0.1/src/corpus_replicator/recipes/audio_flac_flac_libflac.yml
--rw-r--r--   0 worker    (1000) worker    (1000)      900 2023-06-27 18:31:02.000000 corpus-replicator-1.0.1/src/corpus_replicator/recipes/audio_mp3_mp3_libmp3lame.yml
--rw-r--r--   0 worker    (1000) worker    (1000)      337 2023-06-27 18:31:02.000000 corpus-replicator-1.0.1/src/corpus_replicator/recipes/audio_mp3_mp3_shine.yml
--rw-r--r--   0 worker    (1000) worker    (1000)     1107 2023-06-27 18:31:02.000000 corpus-replicator-1.0.1/src/corpus_replicator/recipes/audio_opus_opus_libopus.yml
--rw-r--r--   0 worker    (1000) worker    (1000)      515 2023-06-27 18:31:02.000000 corpus-replicator-1.0.1/src/corpus_replicator/recipes/audio_pcm_wav_ffmpeg.yml
--rw-r--r--   0 worker    (1000) worker    (1000)      481 2023-06-27 18:31:02.000000 corpus-replicator-1.0.1/src/corpus_replicator/recipes/audio_vorbis_ogg_libvorbis.yml
--rw-r--r--   0 worker    (1000) worker    (1000)      610 2023-06-27 18:31:02.000000 corpus-replicator-1.0.1/src/corpus_replicator/recipes/image_bmp_bmp_ffmpeg.yml
--rw-r--r--   0 worker    (1000) worker    (1000)      610 2023-06-27 18:31:02.000000 corpus-replicator-1.0.1/src/corpus_replicator/recipes/image_gif_gif_ffmpeg.yml
--rw-r--r--   0 worker    (1000) worker    (1000)      411 2023-06-27 18:31:02.000000 corpus-replicator-1.0.1/src/corpus_replicator/recipes/image_ico_ico_ffmpeg.yml
--rw-r--r--   0 worker    (1000) worker    (1000)      738 2023-06-27 18:31:02.000000 corpus-replicator-1.0.1/src/corpus_replicator/recipes/image_jpg_jpg_ffmpeg.yml
--rw-r--r--   0 worker    (1000) worker    (1000)      616 2023-06-27 18:31:02.000000 corpus-replicator-1.0.1/src/corpus_replicator/recipes/image_png_png_ffmpeg.yml
--rw-r--r--   0 worker    (1000) worker    (1000)      893 2023-06-27 18:31:02.000000 corpus-replicator-1.0.1/src/corpus_replicator/recipes/image_webp_webp_libwebp.yml
--rw-r--r--   0 worker    (1000) worker    (1000)     1787 2023-06-27 18:31:02.000000 corpus-replicator-1.0.1/src/corpus_replicator/recipes/schema.json
--rw-r--r--   0 worker    (1000) worker    (1000)      654 2023-06-27 18:31:02.000000 corpus-replicator-1.0.1/src/corpus_replicator/recipes/video_av1_webm_libaom.yml
--rw-r--r--   0 worker    (1000) worker    (1000)      713 2023-06-27 18:31:02.000000 corpus-replicator-1.0.1/src/corpus_replicator/recipes/video_h264_mp4_libx264.yml
--rw-r--r--   0 worker    (1000) worker    (1000)      612 2023-06-27 18:31:02.000000 corpus-replicator-1.0.1/src/corpus_replicator/recipes/video_theora_ogg_libtheora.yml
--rw-r--r--   0 worker    (1000) worker    (1000)      617 2023-06-27 18:31:02.000000 corpus-replicator-1.0.1/src/corpus_replicator/recipes/video_vp8_webm_libvpx.yml
--rw-r--r--   0 worker    (1000) worker    (1000)      625 2023-06-27 18:31:02.000000 corpus-replicator-1.0.1/src/corpus_replicator/recipes/video_vp9_webm_libvpx.yml
--rw-r--r--   0 worker    (1000) worker    (1000)      607 2023-06-27 18:31:02.000000 corpus-replicator-1.0.1/src/corpus_replicator/recipes/video_xvid_mp4_libxvid.yml
--rw-r--r--   0 worker    (1000) worker    (1000)    11878 2023-06-27 18:31:02.000000 corpus-replicator-1.0.1/src/corpus_replicator/test_common.py
--rw-r--r--   0 worker    (1000) worker    (1000)     1904 2023-06-27 18:31:02.000000 corpus-replicator-1.0.1/src/corpus_replicator/test_generate_corpus.py
--rw-r--r--   0 worker    (1000) worker    (1000)     2890 2023-06-27 18:31:02.000000 corpus-replicator-1.0.1/src/corpus_replicator/test_generate_template.py
--rw-r--r--   0 worker    (1000) worker    (1000)     4829 2023-06-27 18:31:02.000000 corpus-replicator-1.0.1/src/corpus_replicator/test_replicator.py
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-27 18:31:10.485582 corpus-replicator-1.0.1/src/corpus_replicator/tools/
--rw-r--r--   0 worker    (1000) worker    (1000)        0 2023-06-27 18:31:02.000000 corpus-replicator-1.0.1/src/corpus_replicator/tools/__init__.py
--rw-r--r--   0 worker    (1000) worker    (1000)     1774 2023-06-27 18:31:02.000000 corpus-replicator-1.0.1/src/corpus_replicator/tools/ffmpeg.py
--rw-r--r--   0 worker    (1000) worker    (1000)     1695 2023-06-27 18:31:02.000000 corpus-replicator-1.0.1/src/corpus_replicator/tools/test_ffmpeg.py
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-27 18:31:10.481582 corpus-replicator-1.0.1/src/corpus_replicator.egg-info/
--rw-r--r--   0 worker    (1000) worker    (1000)     2892 2023-06-27 18:31:10.000000 corpus-replicator-1.0.1/src/corpus_replicator.egg-info/PKG-INFO
--rw-r--r--   0 worker    (1000) worker    (1000)     2267 2023-06-27 18:31:10.000000 corpus-replicator-1.0.1/src/corpus_replicator.egg-info/SOURCES.txt
--rw-r--r--   0 worker    (1000) worker    (1000)        1 2023-06-27 18:31:10.000000 corpus-replicator-1.0.1/src/corpus_replicator.egg-info/dependency_links.txt
--rw-r--r--   0 worker    (1000) worker    (1000)       66 2023-06-27 18:31:10.000000 corpus-replicator-1.0.1/src/corpus_replicator.egg-info/entry_points.txt
--rw-r--r--   0 worker    (1000) worker    (1000)        1 2023-06-27 18:31:10.000000 corpus-replicator-1.0.1/src/corpus_replicator.egg-info/not-zip-safe
--rw-r--r--   0 worker    (1000) worker    (1000)       29 2023-06-27 18:31:10.000000 corpus-replicator-1.0.1/src/corpus_replicator.egg-info/requires.txt
--rw-r--r--   0 worker    (1000) worker    (1000)       18 2023-06-27 18:31:10.000000 corpus-replicator-1.0.1/src/corpus_replicator.egg-info/top_level.txt
--rw-r--r--   0 worker    (1000) worker    (1000)     1278 2023-06-27 18:31:02.000000 corpus-replicator-1.0.1/tox.ini
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-07-07 15:49:36.984676 corpus-replicator-1.1.0/
+-rw-r--r--   0 worker    (1000) worker    (1000)      440 2023-07-07 15:49:28.000000 corpus-replicator-1.1.0/.gitignore
+-rw-r--r--   0 worker    (1000) worker    (1000)     2157 2023-07-07 15:49:28.000000 corpus-replicator-1.1.0/.pre-commit-config.yaml
+-rw-r--r--   0 worker    (1000) worker    (1000)     3789 2023-07-07 15:49:28.000000 corpus-replicator-1.1.0/.taskcluster.yml
+-rw-r--r--   0 worker    (1000) worker    (1000)      689 2023-07-07 15:49:28.000000 corpus-replicator-1.1.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 worker    (1000) worker    (1000)    15550 2023-07-07 15:49:28.000000 corpus-replicator-1.1.0/LICENSE.md
+-rw-r--r--   0 worker    (1000) worker    (1000)       44 2023-07-07 15:49:28.000000 corpus-replicator-1.1.0/MANIFEST.in
+-rw-r--r--   0 worker    (1000) worker    (1000)     3734 2023-07-07 15:49:36.984676 corpus-replicator-1.1.0/PKG-INFO
+-rw-r--r--   0 worker    (1000) worker    (1000)     3074 2023-07-07 15:49:28.000000 corpus-replicator-1.1.0/README.md
+-rw-r--r--   0 worker    (1000) worker    (1000)      864 2023-07-07 15:49:28.000000 corpus-replicator-1.1.0/pyproject.toml
+-rw-r--r--   0 worker    (1000) worker    (1000)      976 2023-07-07 15:49:36.984676 corpus-replicator-1.1.0/setup.cfg
+-rwxr-xr-x   0 worker    (1000) worker    (1000)      370 2023-07-07 15:49:28.000000 corpus-replicator-1.1.0/setup.py
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-07-07 15:49:36.968675 corpus-replicator-1.1.0/src/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-07-07 15:49:36.972675 corpus-replicator-1.1.0/src/corpus_replicator/
+-rw-r--r--   0 worker    (1000) worker    (1000)        0 2023-07-07 15:49:28.000000 corpus-replicator-1.1.0/src/corpus_replicator/__init__.py
+-rw-r--r--   0 worker    (1000) worker    (1000)      230 2023-07-07 15:49:28.000000 corpus-replicator-1.1.0/src/corpus_replicator/__main__.py
+-rw-r--r--   0 worker    (1000) worker    (1000)     8358 2023-07-07 15:49:28.000000 corpus-replicator-1.1.0/src/corpus_replicator/common.py
+-rw-r--r--   0 worker    (1000) worker    (1000)    10466 2023-07-07 15:49:28.000000 corpus-replicator-1.1.0/src/corpus_replicator/core.py
+-rw-r--r--   0 worker    (1000) worker    (1000)     3044 2023-07-07 15:49:28.000000 corpus-replicator-1.1.0/src/corpus_replicator/generate_corpus.py
+-rw-r--r--   0 worker    (1000) worker    (1000)     6350 2023-07-07 15:49:28.000000 corpus-replicator-1.1.0/src/corpus_replicator/generate_template.py
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-07-07 15:49:36.980676 corpus-replicator-1.1.0/src/corpus_replicator/recipes/
+-rw-r--r--   0 worker    (1000) worker    (1000)      251 2023-07-07 15:49:28.000000 corpus-replicator-1.1.0/src/corpus_replicator/recipes/animation_apng_png_ffmpeg.yml
+-rw-r--r--   0 worker    (1000) worker    (1000)      216 2023-07-07 15:49:28.000000 corpus-replicator-1.1.0/src/corpus_replicator/recipes/animation_gif_gif_ffmpeg.yml
+-rw-r--r--   0 worker    (1000) worker    (1000)      217 2023-07-07 15:49:28.000000 corpus-replicator-1.1.0/src/corpus_replicator/recipes/animation_webp_webp_libwebp.yml
+-rw-r--r--   0 worker    (1000) worker    (1000)      293 2023-07-07 15:49:28.000000 corpus-replicator-1.1.0/src/corpus_replicator/recipes/audio_aac_mp4_ffmpeg.yml
+-rw-r--r--   0 worker    (1000) worker    (1000)      659 2023-07-07 15:49:28.000000 corpus-replicator-1.1.0/src/corpus_replicator/recipes/audio_flac_flac_libflac.yml
+-rw-r--r--   0 worker    (1000) worker    (1000)      900 2023-07-07 15:49:28.000000 corpus-replicator-1.1.0/src/corpus_replicator/recipes/audio_mp3_mp3_libmp3lame.yml
+-rw-r--r--   0 worker    (1000) worker    (1000)      337 2023-07-07 15:49:28.000000 corpus-replicator-1.1.0/src/corpus_replicator/recipes/audio_mp3_mp3_shine.yml
+-rw-r--r--   0 worker    (1000) worker    (1000)     1107 2023-07-07 15:49:28.000000 corpus-replicator-1.1.0/src/corpus_replicator/recipes/audio_opus_opus_libopus.yml
+-rw-r--r--   0 worker    (1000) worker    (1000)      515 2023-07-07 15:49:28.000000 corpus-replicator-1.1.0/src/corpus_replicator/recipes/audio_pcm_wav_ffmpeg.yml
+-rw-r--r--   0 worker    (1000) worker    (1000)      481 2023-07-07 15:49:28.000000 corpus-replicator-1.1.0/src/corpus_replicator/recipes/audio_vorbis_ogg_libvorbis.yml
+-rw-r--r--   0 worker    (1000) worker    (1000)      436 2023-07-07 15:49:28.000000 corpus-replicator-1.1.0/src/corpus_replicator/recipes/image_avif_avif_imagemagick.yml
+-rw-r--r--   0 worker    (1000) worker    (1000)      610 2023-07-07 15:49:28.000000 corpus-replicator-1.1.0/src/corpus_replicator/recipes/image_bmp_bmp_ffmpeg.yml
+-rw-r--r--   0 worker    (1000) worker    (1000)      610 2023-07-07 15:49:28.000000 corpus-replicator-1.1.0/src/corpus_replicator/recipes/image_gif_gif_ffmpeg.yml
+-rw-r--r--   0 worker    (1000) worker    (1000)      436 2023-07-07 15:49:28.000000 corpus-replicator-1.1.0/src/corpus_replicator/recipes/image_heic_heic_imagemagick.yml
+-rw-r--r--   0 worker    (1000) worker    (1000)      411 2023-07-07 15:49:28.000000 corpus-replicator-1.1.0/src/corpus_replicator/recipes/image_ico_ico_ffmpeg.yml
+-rw-r--r--   0 worker    (1000) worker    (1000)      738 2023-07-07 15:49:28.000000 corpus-replicator-1.1.0/src/corpus_replicator/recipes/image_jpg_jpg_ffmpeg.yml
+-rw-r--r--   0 worker    (1000) worker    (1000)      616 2023-07-07 15:49:28.000000 corpus-replicator-1.1.0/src/corpus_replicator/recipes/image_png_png_ffmpeg.yml
+-rw-r--r--   0 worker    (1000) worker    (1000)      893 2023-07-07 15:49:28.000000 corpus-replicator-1.1.0/src/corpus_replicator/recipes/image_webp_webp_libwebp.yml
+-rw-r--r--   0 worker    (1000) worker    (1000)     1799 2023-07-07 15:49:28.000000 corpus-replicator-1.1.0/src/corpus_replicator/recipes/schema.json
+-rw-r--r--   0 worker    (1000) worker    (1000)      654 2023-07-07 15:49:28.000000 corpus-replicator-1.1.0/src/corpus_replicator/recipes/video_av1_webm_libaom.yml
+-rw-r--r--   0 worker    (1000) worker    (1000)      713 2023-07-07 15:49:28.000000 corpus-replicator-1.1.0/src/corpus_replicator/recipes/video_h264_mp4_libx264.yml
+-rw-r--r--   0 worker    (1000) worker    (1000)      612 2023-07-07 15:49:28.000000 corpus-replicator-1.1.0/src/corpus_replicator/recipes/video_theora_ogg_libtheora.yml
+-rw-r--r--   0 worker    (1000) worker    (1000)      617 2023-07-07 15:49:28.000000 corpus-replicator-1.1.0/src/corpus_replicator/recipes/video_vp8_webm_libvpx.yml
+-rw-r--r--   0 worker    (1000) worker    (1000)      625 2023-07-07 15:49:28.000000 corpus-replicator-1.1.0/src/corpus_replicator/recipes/video_vp9_webm_libvpx.yml
+-rw-r--r--   0 worker    (1000) worker    (1000)      607 2023-07-07 15:49:28.000000 corpus-replicator-1.1.0/src/corpus_replicator/recipes/video_xvid_mp4_libxvid.yml
+-rw-r--r--   0 worker    (1000) worker    (1000)    11878 2023-07-07 15:49:28.000000 corpus-replicator-1.1.0/src/corpus_replicator/test_common.py
+-rw-r--r--   0 worker    (1000) worker    (1000)     1904 2023-07-07 15:49:28.000000 corpus-replicator-1.1.0/src/corpus_replicator/test_generate_corpus.py
+-rw-r--r--   0 worker    (1000) worker    (1000)     2890 2023-07-07 15:49:28.000000 corpus-replicator-1.1.0/src/corpus_replicator/test_generate_template.py
+-rw-r--r--   0 worker    (1000) worker    (1000)     4829 2023-07-07 15:49:28.000000 corpus-replicator-1.1.0/src/corpus_replicator/test_replicator.py
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-07-07 15:49:36.984676 corpus-replicator-1.1.0/src/corpus_replicator/tools/
+-rw-r--r--   0 worker    (1000) worker    (1000)        0 2023-07-07 15:49:28.000000 corpus-replicator-1.1.0/src/corpus_replicator/tools/__init__.py
+-rw-r--r--   0 worker    (1000) worker    (1000)     1775 2023-07-07 15:49:28.000000 corpus-replicator-1.1.0/src/corpus_replicator/tools/ffmpeg.py
+-rw-r--r--   0 worker    (1000) worker    (1000)     1789 2023-07-07 15:49:28.000000 corpus-replicator-1.1.0/src/corpus_replicator/tools/imagemagick.py
+-rw-r--r--   0 worker    (1000) worker    (1000)     1695 2023-07-07 15:49:28.000000 corpus-replicator-1.1.0/src/corpus_replicator/tools/test_ffmpeg.py
+-rw-r--r--   0 worker    (1000) worker    (1000)     1780 2023-07-07 15:49:28.000000 corpus-replicator-1.1.0/src/corpus_replicator/tools/test_imagemagick.py
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-07-07 15:49:36.976676 corpus-replicator-1.1.0/src/corpus_replicator.egg-info/
+-rw-r--r--   0 worker    (1000) worker    (1000)     3734 2023-07-07 15:49:36.000000 corpus-replicator-1.1.0/src/corpus_replicator.egg-info/PKG-INFO
+-rw-r--r--   0 worker    (1000) worker    (1000)     2482 2023-07-07 15:49:36.000000 corpus-replicator-1.1.0/src/corpus_replicator.egg-info/SOURCES.txt
+-rw-r--r--   0 worker    (1000) worker    (1000)        1 2023-07-07 15:49:36.000000 corpus-replicator-1.1.0/src/corpus_replicator.egg-info/dependency_links.txt
+-rw-r--r--   0 worker    (1000) worker    (1000)       66 2023-07-07 15:49:36.000000 corpus-replicator-1.1.0/src/corpus_replicator.egg-info/entry_points.txt
+-rw-r--r--   0 worker    (1000) worker    (1000)        1 2023-07-07 15:49:36.000000 corpus-replicator-1.1.0/src/corpus_replicator.egg-info/not-zip-safe
+-rw-r--r--   0 worker    (1000) worker    (1000)       29 2023-07-07 15:49:36.000000 corpus-replicator-1.1.0/src/corpus_replicator.egg-info/requires.txt
+-rw-r--r--   0 worker    (1000) worker    (1000)       18 2023-07-07 15:49:36.000000 corpus-replicator-1.1.0/src/corpus_replicator.egg-info/top_level.txt
+-rw-r--r--   0 worker    (1000) worker    (1000)     1278 2023-07-07 15:49:28.000000 corpus-replicator-1.1.0/tox.ini
```

### Comparing `corpus-replicator-1.0.1/.pre-commit-config.yaml` & `corpus-replicator-1.1.0/.pre-commit-config.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,15 @@
         types: [yaml]
         args: ["--schemafile", "./src/corpus_replicator/recipes/schema.json"]
   - repo: https://github.com/marco-c/taskcluster_yml_validator
     rev: v0.0.10
     hooks:
       - id: taskcluster_yml
   - repo: https://github.com/MozillaSecurity/orion
-    rev: v0.0.6
+    rev: v0.0.7
     hooks:
       - id: orion_ci
   - repo: meta
     hooks:
       - id: check-useless-excludes
   - repo: local
     hooks:
```

### Comparing `corpus-replicator-1.0.1/.taskcluster.yml` & `corpus-replicator-1.1.0/.taskcluster.yml`

 * *Files identical despite different names*

### Comparing `corpus-replicator-1.0.1/CODE_OF_CONDUCT.md` & `corpus-replicator-1.1.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `corpus-replicator-1.0.1/LICENSE.md` & `corpus-replicator-1.1.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `corpus-replicator-1.0.1/PKG-INFO` & `corpus-replicator-1.1.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,46 +1,36 @@
-Metadata-Version: 2.1
-Name: corpus-replicator
-Version: 1.0.1
-Home-page: https://github.com/MozillaSecurity/corpus-replicator
-Author: Tyson Smith
-Author-email: twsmith@mozilla.com
-Maintainer: Mozilla Fuzzing Team
-Maintainer-email: fuzzing@mozilla.com
-License: MPL 2.0
-Keywords: automation corpus fuzz fuzzing security test testing
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
-Classifier: Programming Language :: Python :: 3
-Classifier: Topic :: Software Development :: Testing
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE.md
-
 Corpus Replicator
 =================
+[![Task Status](https://community-tc.services.mozilla.com/api/github/v1/repository/MozillaSecurity/corpus-replicator/main/badge.svg)](https://community-tc.services.mozilla.com/api/github/v1/repository/MozillaSecurity/corpus-replicator/main/latest)
+[![Matrix](https://img.shields.io/badge/dynamic/json?color=green&label=chat&query=%24.chunk[%3F(%40.canonical_alias%3D%3D%22%23fuzzing%3Amozilla.org%22)].num_joined_members&suffix=%20users&url=https%3A%2F%2Fmozilla.modular.im%2F_matrix%2Fclient%2Fr0%2FpublicRooms&style=flat&logo=matrix)](https://riot.im/app/#/room/#fuzzing:mozilla.org)
+[![PyPI](https://img.shields.io/pypi/v/corpus-replicator)](https://pypi.org/project/corpus-replicator)
 
 Corpus Replicator is a corpus generation tool that enables the creation of multiple
 unique output files based on templates. The primary intended use case is the
 creation of a seed corpus that can be used by fuzzers. Support for additional output
 formats can be added via the creation of `Recipes`. If a desired format is unsupported,
 support can be added via the creation of a `CorpusGenerator`.
 
 The goal is to create an efficient corpus that maximizes code coverage and minimizes
 file size. Small unique files that execute quickly are preferred.
 
-Currently four media types can be generated `animations`, `audio`, `images` and
-`videos`.
+Currently four media types can be generated `animation`, `audio`, `image` and
+`video`.
 
 Requirements
 ------------
 
 Corpus Replicator relies on [FFmpeg](https://ffmpeg.org/).
 
+Installation
+------------
+```
+pip install corpus-replicator
+```
+
 Example
 -------
 
 This is an example `recipe` file.
 
 ```yaml
 # "base" contains required entries and default flags
@@ -63,15 +53,15 @@
   - ["-s", "640x480"]
   - ["-s", "32x18"]
   - ["-s", "64x64"]
   monochrome:         # flag group - adds new flag group
   - ["-vf", "monochrome"]
 ```
 
-Running the recipe to generate a corpus:
+Running the recipe will generate a corpus:
 ```
 $ corpus-replicator example.yml video -t test
 Generating templates...
 1 recipe(s) will be used with 1 template(s) to create 4 file(s).
 Generating 4 'video/libx264/h264/mp4' file(s) using template 'test'...
 Optimizing corpus, checking for duplicates...
 Done.
@@ -84,7 +74,9 @@
 video-h264-libx264-test-resolution-01.mp4
 video-h264-libx264-test-resolution-00.mp4
 video-h264-libx264-test-resolution-02.mp4
 ```
 
 A more complex corpus can be generated by using multiple `Recipes` and `Templates` at
 once.
+
+Recipes are stored in [src/corpus_replicator/recipes](/src/corpus_replicator/recipes/).
```

### Comparing `corpus-replicator-1.0.1/pyproject.toml` & `corpus-replicator-1.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `corpus-replicator-1.0.1/setup.cfg` & `corpus-replicator-1.1.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `corpus-replicator-1.0.1/src/corpus_replicator/common.py` & `corpus-replicator-1.1.0/src/corpus_replicator/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from subprocess import run
 from typing import Any, Dict, Iterator, List, Tuple
 
 from yaml import YAMLError, safe_load
 
 LOG = getLogger(__name__)
 SUPPORTED_MEDIUM = ("animation", "audio", "image", "video")
-SUPPORTED_TOOLS = ("ffmpeg",)
+SUPPORTED_TOOLS = ("ffmpeg", "imagemagick")
 TOOL_LOG: str = "replicator-tool-log.txt"
 
 
 class RecipeError(Exception):
     """Recipe related errors."""
```

### Comparing `corpus-replicator-1.0.1/src/corpus_replicator/core.py` & `corpus-replicator-1.1.0/src/corpus_replicator/core.py`

 * *Files identical despite different names*

### Comparing `corpus-replicator-1.0.1/src/corpus_replicator/generate_corpus.py` & `corpus-replicator-1.1.0/src/corpus_replicator/generate_corpus.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,35 +2,40 @@
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at http://mozilla.org/MPL/2.0/.
 from argparse import ArgumentParser, Namespace
 from logging import DEBUG, INFO, getLogger
 from pathlib import Path
 from typing import List, Optional
 
-from .common import Recipe, Template, ToolError, init_logging
+from .common import CorpusGenerator, Recipe, Template, ToolError, init_logging
 from .tools.ffmpeg import FFmpegGenerator, ffmpeg_available
+from .tools.imagemagick import ImageMagickGenerator, imagemagick_available
 
 LOG = getLogger(__name__)
 
 
-def load_generator(recipe: Recipe, dest: Path) -> FFmpegGenerator:
+def load_generator(recipe: Recipe, dest: Path) -> CorpusGenerator:
     """Load a specific generator to use to create the corpus.
 
     Args:
         recipe: Recipe to use to generate corpus.
         dest: Location to place generated corpus.
 
     Returns:
         A corpus generator.
     """
-    generator: Optional[FFmpegGenerator] = None
+    generator: Optional[CorpusGenerator] = None
     if recipe.tool == "ffmpeg":
         if not ffmpeg_available():
             raise ToolError("FFmpeg is not available")
         generator = FFmpegGenerator(recipe, dest)
+    elif recipe.tool == "imagemagick":
+        if not imagemagick_available():
+            raise ToolError("ImageMagick is not available")
+        generator = ImageMagickGenerator(recipe, dest)
     else:
         raise ToolError(f"Unsupported tool {recipe.tool!r}")
     assert generator is not None
     return generator
 
 
 def main(argv: Optional[List[str]] = None) -> None:
```

### Comparing `corpus-replicator-1.0.1/src/corpus_replicator/generate_template.py` & `corpus-replicator-1.1.0/src/corpus_replicator/generate_template.py`

 * *Files identical despite different names*

### Comparing `corpus-replicator-1.0.1/src/corpus_replicator/recipes/audio_flac_flac_libflac.yml` & `corpus-replicator-1.1.0/src/corpus_replicator/recipes/audio_flac_flac_libflac.yml`

 * *Files identical despite different names*

### Comparing `corpus-replicator-1.0.1/src/corpus_replicator/recipes/audio_mp3_mp3_libmp3lame.yml` & `corpus-replicator-1.1.0/src/corpus_replicator/recipes/audio_mp3_mp3_libmp3lame.yml`

 * *Files identical despite different names*

### Comparing `corpus-replicator-1.0.1/src/corpus_replicator/recipes/audio_opus_opus_libopus.yml` & `corpus-replicator-1.1.0/src/corpus_replicator/recipes/audio_opus_opus_libopus.yml`

 * *Files identical despite different names*

### Comparing `corpus-replicator-1.0.1/src/corpus_replicator/recipes/audio_pcm_wav_ffmpeg.yml` & `corpus-replicator-1.1.0/src/corpus_replicator/recipes/audio_pcm_wav_ffmpeg.yml`

 * *Files identical despite different names*

### Comparing `corpus-replicator-1.0.1/src/corpus_replicator/recipes/image_bmp_bmp_ffmpeg.yml` & `corpus-replicator-1.1.0/src/corpus_replicator/recipes/image_bmp_bmp_ffmpeg.yml`

 * *Files identical despite different names*

### Comparing `corpus-replicator-1.0.1/src/corpus_replicator/recipes/image_gif_gif_ffmpeg.yml` & `corpus-replicator-1.1.0/src/corpus_replicator/recipes/image_gif_gif_ffmpeg.yml`

 * *Files identical despite different names*

### Comparing `corpus-replicator-1.0.1/src/corpus_replicator/recipes/image_jpg_jpg_ffmpeg.yml` & `corpus-replicator-1.1.0/src/corpus_replicator/recipes/image_jpg_jpg_ffmpeg.yml`

 * *Files identical despite different names*

### Comparing `corpus-replicator-1.0.1/src/corpus_replicator/recipes/image_png_png_ffmpeg.yml` & `corpus-replicator-1.1.0/src/corpus_replicator/recipes/image_png_png_ffmpeg.yml`

 * *Files identical despite different names*

### Comparing `corpus-replicator-1.0.1/src/corpus_replicator/recipes/image_webp_webp_libwebp.yml` & `corpus-replicator-1.1.0/src/corpus_replicator/recipes/image_webp_webp_libwebp.yml`

 * *Files identical despite different names*

### Comparing `corpus-replicator-1.0.1/src/corpus_replicator/recipes/schema.json` & `corpus-replicator-1.1.0/src/corpus_replicator/recipes/schema.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999457465277778%*

 * *Differences: {"'properties'": "{'base': {'properties': {'tool': {'pattern': 'ffmpeg|imagemagick'}}}}"}*

```diff
@@ -33,15 +33,15 @@
                     "type": "string"
                 },
                 "medium": {
                     "pattern": "animation|audio|image|video",
                     "type": "string"
                 },
                 "tool": {
-                    "pattern": "ffmpeg",
+                    "pattern": "ffmpeg|imagemagick",
                     "type": "string"
                 }
             },
             "required": [
                 "codec",
                 "container",
                 "library",
```

### Comparing `corpus-replicator-1.0.1/src/corpus_replicator/recipes/video_av1_webm_libaom.yml` & `corpus-replicator-1.1.0/src/corpus_replicator/recipes/video_av1_webm_libaom.yml`

 * *Files identical despite different names*

### Comparing `corpus-replicator-1.0.1/src/corpus_replicator/recipes/video_h264_mp4_libx264.yml` & `corpus-replicator-1.1.0/src/corpus_replicator/recipes/video_h264_mp4_libx264.yml`

 * *Files identical despite different names*

### Comparing `corpus-replicator-1.0.1/src/corpus_replicator/recipes/video_theora_ogg_libtheora.yml` & `corpus-replicator-1.1.0/src/corpus_replicator/recipes/video_theora_ogg_libtheora.yml`

 * *Files identical despite different names*

### Comparing `corpus-replicator-1.0.1/src/corpus_replicator/recipes/video_vp8_webm_libvpx.yml` & `corpus-replicator-1.1.0/src/corpus_replicator/recipes/video_vp8_webm_libvpx.yml`

 * *Files identical despite different names*

### Comparing `corpus-replicator-1.0.1/src/corpus_replicator/recipes/video_vp9_webm_libvpx.yml` & `corpus-replicator-1.1.0/src/corpus_replicator/recipes/video_vp9_webm_libvpx.yml`

 * *Files identical despite different names*

### Comparing `corpus-replicator-1.0.1/src/corpus_replicator/recipes/video_xvid_mp4_libxvid.yml` & `corpus-replicator-1.1.0/src/corpus_replicator/recipes/video_xvid_mp4_libxvid.yml`

 * *Files identical despite different names*

### Comparing `corpus-replicator-1.0.1/src/corpus_replicator/test_common.py` & `corpus-replicator-1.1.0/src/corpus_replicator/test_common.py`

 * *Files identical despite different names*

### Comparing `corpus-replicator-1.0.1/src/corpus_replicator/test_generate_corpus.py` & `corpus-replicator-1.1.0/src/corpus_replicator/test_generate_corpus.py`

 * *Files identical despite different names*

### Comparing `corpus-replicator-1.0.1/src/corpus_replicator/test_generate_template.py` & `corpus-replicator-1.1.0/src/corpus_replicator/test_generate_template.py`

 * *Files identical despite different names*

### Comparing `corpus-replicator-1.0.1/src/corpus_replicator/test_replicator.py` & `corpus-replicator-1.1.0/src/corpus_replicator/test_replicator.py`

 * *Files identical despite different names*

### Comparing `corpus-replicator-1.0.1/src/corpus_replicator/tools/ffmpeg.py` & `corpus-replicator-1.1.0/src/corpus_replicator/tools/imagemagick.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,53 +3,53 @@
 # file, You can obtain one at http://mozilla.org/MPL/2.0/.
 from pathlib import Path
 from shutil import which
 from typing import Iterator
 
 from ..common import CorpusGenerator, run_tool
 
-FFMPEG_BIN = "ffmpeg"
+IMAGEMAGICK_BIN = "convert"
 
 
-class FFmpegGenerator(CorpusGenerator):
-    """FFmpeg wrapper."""
+class ImageMagickGenerator(CorpusGenerator):
+    """ImageMagick wrapper."""
 
     def generate(self) -> Iterator[Path]:
         """Generate corpus. Templates are combined with Recipes to create variations
         based on parameters defined in the Recipes.
 
         Args:
             recipe: Recipe to use to generate a corpus.
             dest: Location to place generated corpus.
 
         Yields:
             A corpus generator.
         """
         for template in self._templates:
-            base_cmd = [FFMPEG_BIN, "-i", str(template.file), "-y"]
+            base_cmd = [IMAGEMAGICK_BIN, str(template.file)]
             for flag, idx, variation in self._recipe:
-                # build dest file name 'video-h264-library-noise-resolution-##.mp4'
+                # build dest file name 'img-jpeg-library-noise-resolution-##.mp4'
                 dest_file = self._dest / "-".join(
                     [
                         self._recipe.medium,
                         self._recipe.codec,
                         self._recipe.library,
                         template.name,
                         flag,
                         f"{idx:02d}.{self._recipe.container}",
                     ]
                 )
                 run_tool(base_cmd + variation + [str(dest_file)])
                 yield dest_file
 
 
-def ffmpeg_available() -> bool:
-    """Check FFmpeg if is installed.
+def imagemagick_available() -> bool:
+    """Check if ImageMagick is installed.
 
     Args:
         None
 
     Return:
-        True if FFmpeg installed otherwise False.
+        True if installed otherwise False.
     """
     # TODO: check version and flags for available features?
-    return which(FFMPEG_BIN) is not None
+    return which(IMAGEMAGICK_BIN) is not None
```

### Comparing `corpus-replicator-1.0.1/src/corpus_replicator/tools/test_ffmpeg.py` & `corpus-replicator-1.1.0/src/corpus_replicator/tools/test_ffmpeg.py`

 * *Files identical despite different names*

### Comparing `corpus-replicator-1.0.1/src/corpus_replicator.egg-info/SOURCES.txt` & `corpus-replicator-1.1.0/src/corpus_replicator.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -32,23 +32,27 @@
 src/corpus_replicator/recipes/audio_aac_mp4_ffmpeg.yml
 src/corpus_replicator/recipes/audio_flac_flac_libflac.yml
 src/corpus_replicator/recipes/audio_mp3_mp3_libmp3lame.yml
 src/corpus_replicator/recipes/audio_mp3_mp3_shine.yml
 src/corpus_replicator/recipes/audio_opus_opus_libopus.yml
 src/corpus_replicator/recipes/audio_pcm_wav_ffmpeg.yml
 src/corpus_replicator/recipes/audio_vorbis_ogg_libvorbis.yml
+src/corpus_replicator/recipes/image_avif_avif_imagemagick.yml
 src/corpus_replicator/recipes/image_bmp_bmp_ffmpeg.yml
 src/corpus_replicator/recipes/image_gif_gif_ffmpeg.yml
+src/corpus_replicator/recipes/image_heic_heic_imagemagick.yml
 src/corpus_replicator/recipes/image_ico_ico_ffmpeg.yml
 src/corpus_replicator/recipes/image_jpg_jpg_ffmpeg.yml
 src/corpus_replicator/recipes/image_png_png_ffmpeg.yml
 src/corpus_replicator/recipes/image_webp_webp_libwebp.yml
 src/corpus_replicator/recipes/schema.json
 src/corpus_replicator/recipes/video_av1_webm_libaom.yml
 src/corpus_replicator/recipes/video_h264_mp4_libx264.yml
 src/corpus_replicator/recipes/video_theora_ogg_libtheora.yml
 src/corpus_replicator/recipes/video_vp8_webm_libvpx.yml
 src/corpus_replicator/recipes/video_vp9_webm_libvpx.yml
 src/corpus_replicator/recipes/video_xvid_mp4_libxvid.yml
 src/corpus_replicator/tools/__init__.py
 src/corpus_replicator/tools/ffmpeg.py
-src/corpus_replicator/tools/test_ffmpeg.py
+src/corpus_replicator/tools/imagemagick.py
+src/corpus_replicator/tools/test_ffmpeg.py
+src/corpus_replicator/tools/test_imagemagick.py
```

### Comparing `corpus-replicator-1.0.1/tox.ini` & `corpus-replicator-1.1.0/tox.ini`

 * *Files identical despite different names*

