# Comparing `tmp/duplipy-0.1.5.tar.gz` & `tmp/duplipy-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "duplipy-0.1.5.tar", last modified: Fri Jul  7 12:58:31 2023, max compression
+gzip compressed data, was "duplipy-0.1.6.tar", last modified: Fri Jul  7 14:33:03 2023, max compression
```

## Comparing `duplipy-0.1.5.tar` & `duplipy-0.1.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-07-07 12:58:31.324668 duplipy-0.1.5/
--rw-rw-rw-   0        0        0      955 2023-07-07 06:34:30.000000 duplipy-0.1.5/LICENSE
--rw-rw-rw-   0        0        0      941 2023-07-07 12:58:31.321672 duplipy-0.1.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-07 12:58:31.286672 duplipy-0.1.5/duplipy/
--rw-rw-rw-   0        0        0      618 2023-07-07 12:56:20.000000 duplipy-0.1.5/duplipy/__init__.py
--rw-rw-rw-   0        0        0     6539 2023-07-07 08:39:46.000000 duplipy-0.1.5/duplipy/formatting.py
--rw-rw-rw-   0        0        0     8392 2023-07-07 09:09:32.000000 duplipy-0.1.5/duplipy/replication.py
--rw-rw-rw-   0        0        0     2676 2023-07-07 09:14:40.000000 duplipy-0.1.5/duplipy/similarity.py
--rw-rw-rw-   0        0        0     2305 2023-07-07 09:23:12.000000 duplipy-0.1.5/duplipy/text_analysis.py
-drwxrwxrwx   0        0        0        0 2023-07-07 12:58:31.311672 duplipy-0.1.5/duplipy.egg-info/
--rw-rw-rw-   0        0        0      941 2023-07-07 12:58:31.000000 duplipy-0.1.5/duplipy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      282 2023-07-07 12:58:31.000000 duplipy-0.1.5/duplipy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-07 12:58:31.000000 duplipy-0.1.5/duplipy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       64 2023-07-07 12:58:31.000000 duplipy-0.1.5/duplipy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-07-07 12:58:31.000000 duplipy-0.1.5/duplipy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-07 12:58:31.325670 duplipy-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0     1264 2023-07-07 12:58:19.000000 duplipy-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-07 14:33:03.526834 duplipy-0.1.6/
+-rw-rw-rw-   0        0        0      955 2023-07-07 06:34:30.000000 duplipy-0.1.6/LICENSE
+-rw-rw-rw-   0        0        0      941 2023-07-07 14:33:03.524830 duplipy-0.1.6/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-07 14:33:03.487832 duplipy-0.1.6/duplipy/
+-rw-rw-rw-   0        0        0      524 2023-07-07 14:21:00.000000 duplipy-0.1.6/duplipy/__init__.py
+-rw-rw-rw-   0        0        0     6539 2023-07-07 08:39:46.000000 duplipy-0.1.6/duplipy/formatting.py
+-rw-rw-rw-   0        0        0     7545 2023-07-07 13:11:20.000000 duplipy-0.1.6/duplipy/replication.py
+-rw-rw-rw-   0        0        0     1533 2023-07-07 14:20:43.000000 duplipy-0.1.6/duplipy/similarity.py
+-rw-rw-rw-   0        0        0      897 2023-07-07 14:21:51.000000 duplipy-0.1.6/duplipy/text_analysis.py
+drwxrwxrwx   0        0        0        0 2023-07-07 14:33:03.519834 duplipy-0.1.6/duplipy.egg-info/
+-rw-rw-rw-   0        0        0      941 2023-07-07 14:33:02.000000 duplipy-0.1.6/duplipy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      282 2023-07-07 14:33:03.000000 duplipy-0.1.6/duplipy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-07 14:33:02.000000 duplipy-0.1.6/duplipy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       33 2023-07-07 14:33:02.000000 duplipy-0.1.6/duplipy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-07 14:33:02.000000 duplipy-0.1.6/duplipy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-07 14:33:03.527843 duplipy-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0     1197 2023-07-07 14:18:07.000000 duplipy-0.1.6/setup.py
```

### Comparing `duplipy-0.1.5/LICENSE` & `duplipy-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `duplipy-0.1.5/PKG-INFO` & `duplipy-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: duplipy
-Version: 0.1.5
+Version: 0.1.6
 Summary: A package for formatting and text replication.
 Home-page: https://github.com/infinitode/duplipy
 Author: Infinitode Pty Ltd
 Author-email: infinitode.ltd@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `duplipy-0.1.5/duplipy/__init__.py` & `duplipy-0.1.6/duplipy/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,5 +1,5 @@
 import duplipy
 from .formatting import remove_stopwords, remove_numbers, remove_whitespace, normalize_whitespace, separate_symbols, remove_special_characters, standardize_text, tokenize_text, stem_words, lemmatize_words, pos_tag
-from .replication import replace_word_with_synonym, augment_text_with_synonyms, load_text_file, augment_file_with_synonyms, backtranslate, insert_random_word, delete_random_word, insert_synonym, paraphrase
-from .similarity import cosine_similarity_score, jaccard_similarity_score, edit_distance_score
-from .text_analysis import extract_named_entities, translate_text, analyze_sentiment
+from .replication import replace_word_with_synonym, augment_text_with_synonyms, load_text_file, augment_file_with_synonyms, insert_random_word, delete_random_word, insert_synonym, paraphrase
+from .similarity import edit_distance_score, bleu_score
+from .text_analysis import analyze_sentiment
```

### Comparing `duplipy-0.1.5/duplipy/formatting.py` & `duplipy-0.1.6/duplipy/formatting.py`

 * *Files identical despite different names*

### Comparing `duplipy-0.1.5/duplipy/replication.py` & `duplipy-0.1.6/duplipy/replication.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,26 +2,24 @@
 Text replication for NLP.
 
 Available functions:
 - `replace_word_with_synonym(word)`: Replace the given word with a synonym.
 - `augment_text_with_synonyms(text, augmentation_factor, probability, progress=True)`: Augment the input text by replacing words with synonyms.
 - `load_text_file(filepath)`: Load the contents of a text file.
 - `augment_file_with_synonyms(file_path, augmentation_factor, probability, progress=True)`: Augment a text file by replacing words with synonyms.
-- `backtranslate(text, target_language='en')`: Perform backtranslation on the input text.
 - `insert_random_word(text, word)`: Insert a random word into the input text.
 - `delete_random_word(text)`: Delete a random word from the input text.
 - `insert_synonym(text, word)`: Insert a synonym of the given word into the input text.
 - `paraphrase(text)`: Paraphrase the input text.
 """
 
 import random
 import time
 import nltk
 from nltk.corpus import wordnet
-from nltk.translate import Translator
 
 nltk.download("wordnet", quiet=True)
 nltk.download("averaged_perceptron_tagger", quiet=True)
 nltk.download("punkt", quiet=True)
 
 def replace_word_with_synonym(word):
     """
@@ -140,34 +138,14 @@
         text = load_text_file(file_path)
         augmented_text = augment_text_with_synonyms(text, augmentation_factor, probability, progress)
         return augmented_text
     except Exception as e:
         print(f"An error occurred during text file augmentation: {str(e)}")
         return []
 
-def backtranslate(text, target_language="en"):
-    """
-    Perform backtranslation on the input text.
-
-    Parameters:
-    - `text` (str): The input text to be backtranslated.
-    - `target_language` (str): The target language to translate the text into. Default is "en".
-
-    Returns:
-    - `str`: The backtranslated text.
-    """
-    try:
-        translator = Translator()
-        translated_text = translator.translate(text, dest=target_language).text
-        backtranslated_text = translator.translate(translated_text, dest="original").text
-        return backtranslated_text
-    except Exception as e:
-        print(f"An error occurred during backtranslation: {str(e)}")
-        return text
-
 
 def insert_random_word(text, word):
     """
     Insert a random word into the input text.
 
     Parameters:
     - `text` (str): The input text for word insertion.
```

### Comparing `duplipy-0.1.5/duplipy.egg-info/PKG-INFO` & `duplipy-0.1.6/duplipy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: duplipy
-Version: 0.1.5
+Version: 0.1.6
 Summary: A package for formatting and text replication.
 Home-page: https://github.com/infinitode/duplipy
 Author: Infinitode Pty Ltd
 Author-email: infinitode.ltd@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `duplipy-0.1.5/setup.py` & `duplipy-0.1.6/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,24 @@
 from setuptools import setup, find_packages
 
 setup(
     name='duplipy',
-    version='0.1.5',
+    version='0.1.6',
     author='Infinitode Pty Ltd',
     author_email='infinitode.ltd@gmail.com',
     description='A package for formatting and text replication.',
     long_description='DupliPy is a quick and easy-to-use package that can handle text formatting and data augmentation tasks for NLP in Python.',
     long_description_content_type='text/markdown',
     url='https://github.com/infinitode/duplipy',
     packages=find_packages(),
     install_requires=[
         'nltk',
         'numpy',
-        'spacy',
         'langcodes',
-        'googletrans',
         'joblib',
-        'scikit-learn',
         'tqdm',
     ],
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
```

