# Comparing `tmp/doctran-0.0.2.tar.gz` & `tmp/doctran-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "doctran-0.0.2.tar", max compression
+gzip compressed data, was "doctran-0.0.3.tar", max compression
```

## Comparing `doctran-0.0.2.tar` & `doctran-0.0.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1064 2023-06-24 22:31:03.176553 doctran-0.0.2/LICENSE
--rw-r--r--   0        0        0     8028 2023-07-02 17:43:40.049930 doctran-0.0.2/README.md
--rw-r--r--   0        0        0      117 2023-07-02 00:38:58.942692 doctran-0.0.2/doctran/__init__.py
--rw-r--r--   0        0        0     7684 2023-07-07 17:58:31.686595 doctran-0.0.2/doctran/doctran.py
--rw-r--r--   0        0        0      175 2023-07-01 18:30:41.396740 doctran-0.0.2/doctran/transformers/__init__.py
--rw-r--r--   0        0        0      413 2023-07-01 18:31:07.391598 doctran-0.0.2/doctran/transformers/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     8900 2023-06-30 02:26:08.286700 doctran-0.0.2/doctran/transformers/__pycache__/document_transformers.cpython-310.pyc
--rw-r--r--   0        0        0      462 2023-06-29 15:35:41.652339 doctran-0.0.2/doctran/transformers/__pycache__/prompts.cpython-310.pyc
--rw-r--r--   0        0        0    10879 2023-07-02 01:44:18.224865 doctran-0.0.2/doctran/transformers/__pycache__/transformers.cpython-310.pyc
--rw-r--r--   0        0        0    12122 2023-07-02 01:43:59.344967 doctran-0.0.2/doctran/transformers/transformers.py
--rw-r--r--   0        0        0      684 2023-07-07 18:00:27.310514 doctran-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     8930 1970-01-01 00:00:00.000000 doctran-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-06-24 22:31:03.176553 doctran-0.0.3/LICENSE
+-rw-r--r--   0        0        0     8124 2023-07-07 20:26:59.304557 doctran-0.0.3/README.md
+-rw-r--r--   0        0        0      117 2023-07-02 00:38:58.942692 doctran-0.0.3/doctran/__init__.py
+-rw-r--r--   0        0        0     7658 2023-07-07 20:36:08.795957 doctran-0.0.3/doctran/doctran.py
+-rw-r--r--   0        0        0      175 2023-07-01 18:30:41.396740 doctran-0.0.3/doctran/transformers/__init__.py
+-rw-r--r--   0        0        0      413 2023-07-01 18:31:07.391598 doctran-0.0.3/doctran/transformers/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     8900 2023-06-30 02:26:08.286700 doctran-0.0.3/doctran/transformers/__pycache__/document_transformers.cpython-310.pyc
+-rw-r--r--   0        0        0      462 2023-06-29 15:35:41.652339 doctran-0.0.3/doctran/transformers/__pycache__/prompts.cpython-310.pyc
+-rw-r--r--   0        0        0    10879 2023-07-02 01:44:18.224865 doctran-0.0.3/doctran/transformers/__pycache__/transformers.cpython-310.pyc
+-rw-r--r--   0        0        0    12106 2023-07-07 20:34:46.888870 doctran-0.0.3/doctran/transformers/transformers.py
+-rw-r--r--   0        0        0      586 2023-07-07 20:35:12.430312 doctran-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     8824 1970-01-01 00:00:00.000000 doctran-0.0.3/PKG-INFO
```

### Comparing `doctran-0.0.2/LICENSE` & `doctran-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `doctran-0.0.2/README.md` & `doctran-0.0.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -2,30 +2,30 @@
 🐛 Doctran
 </h2>
 
 <p align="center">
   <p align="center"><b>Doc</b>ument <b>tran</b>sformation framework to improve vector search results</p>
 </p>
 <p align="center">
-<a href="https://join.slack.com/t/psychicapi/shared_invite/zt-1ty1wz6w0-8jkmdvBpM5kj_Fh30EiCcg" target="_blank">
+<a href="https://join.slack.com/t/psychicapi/shared_invite/zt-1yptnhwcz-SiOCnrbqnBDsuzps9sEMSw" target="_blank">
     <img src="https://img.shields.io/badge/slack-join-blue.svg?logo=slack" alt="Slack">
 </a>
 </a>
 <a href="https://github.com/psychic-api/doctran/blob/main/LICENSE" target="_blank">
     <img src="https://img.shields.io/static/v1?label=license&message=MIT&color=blue" alt="License">
 </a>
 <a href="https://github.com/psychic-api/doctran/issues" target="_blank">
     <img src="https://img.shields.io/github/issues/psychic-api/doctran?color=blue" alt="Issues">
 </a>
   <a href="https://twitter.com/psychicapi" target="_blank">
     <img src="https://img.shields.io/twitter/follow/psychicapi?style=social" alt="Twitter">
 </a>
 </p>
 
-Vector databases are useful for retrieving context for LLMs, however they struggle to find relevant information if the source documents are indexed hapharzardly and information is sparse. Doctran uses LLMs and open source NLP libraries to transform raw text into clean, structured, information-dense documents that are optimized for vector space retrieval.
+Vector databases are useful for retrieving context for LLMs, however they struggle to find relevant information if the source documents are indexed hapharzardly and information is sparse. Doctran uses LLMs and open source NLP libraries to transform raw text into clean, structured, information-dense documents that are optimized for vector space retrieval. You can think of Doctran as a black box where messy strings go in and nice, clean, labelled strings come out.
 
 Doctran is maintained by [Psychic](https://github.com/psychic-api/psychic), the data integration layer for LLMs.
 
 ## Examples
 Clone or download [`examples.ipynb`](/examples.ipynb) for interactive demos.
 
 #### Doctran converts messy, unstructured text
@@ -44,15 +44,15 @@
 </section>
 <section>
 <header>HR Updates and Employee Benefits</header>
 <p>Recently, we welcomed several new team members who have made significant contributions to their respective departments. I would like to recognize Jane Smith (SSN: &#x0030; &#x0034; &#x0039; - &#x0034; &#x0035; - &#x0035; &#x0039; &#x0032; &#x0038;) for her outstanding performance in customer service. Jane has consistently received positive feedback from our clients. Furthermore, please remember that the open enrollment period for our employee benefits program is fast approaching. Should you have any questions or require assistance, please contact our HR representative, Michael Johnson (phone: &#x0034; &#x0031; 
 ...
 ```
 
-#### Into structured or semi-structured documents that are optimized for vector search.
+#### Into semi-structured documents that are optimized for vector search.
 
 ```
 {
   "topics": ["Security and Privacy", "HR Updates", "Marketing", "R&D"],
   "summary": "The document discusses updates on security measures, HR, marketing initiatives, and R&D projects. It commends John Doe for enhancing network security, welcomes new team members, and recognizes Jane Smith for her customer service. It also mentions the open enrollment period for employee benefits, thanks Sarah Thompson for her social media efforts, and announces a product launch event on July 15th. David Rodriguez is acknowledged for his contributions to R&D. The document emphasizes the importance of confidentiality.",
   "contact_info": [
     {
@@ -108,15 +108,15 @@
 ```python
 document = await document.redact(entities=["EMAIL_ADDRESS", "PHONE_NUMBER"]).extract(properties).summarize().execute()
 ```
 
 ## Doctransformers
 
 ### Extract
-Given any valid JSON schema, yses OpenAI function calling to extract structured data from a document.
+Given any valid JSON schema, uses OpenAI function calling to extract structured data from a document.
 
 ```python
 from doctran import ExtractProperty
 
 properties = ExtractProperty(
     name="millenial_or_boomer", 
     description="A prediction of whether this document was written by a millenial or boomer",
```

#### html2text {}

```diff
@@ -2,21 +2,22 @@
       Document transformation framework to improve vector search results
                                     [Slack]
  [License] [Issues] [Twitter]
 Vector databases are useful for retrieving context for LLMs, however they
 struggle to find relevant information if the source documents are indexed
 hapharzardly and information is sparse. Doctran uses LLMs and open source NLP
 libraries to transform raw text into clean, structured, information-dense
-documents that are optimized for vector space retrieval. Doctran is maintained
-by [Psychic](https://github.com/psychic-api/psychic), the data integration
-layer for LLMs. ## Examples Clone or download [`examples.ipynb`](/
-examples.ipynb) for interactive demos. #### Doctran converts messy,
-unstructured text ```    &#x004A; &#x0075; &#x006C; &#x0079; &#x0020; &#x0031;
-, &#x0032; &#x0030; &#x0032; &#x0033;   Updates and Discussions on Various
-Topics;
+documents that are optimized for vector space retrieval. You can think of
+Doctran as a black box where messy strings go in and nice, clean, labelled
+strings come out. Doctran is maintained by [Psychic](https://github.com/
+psychic-api/psychic), the data integration layer for LLMs. ## Examples Clone or
+download [`examples.ipynb`](/examples.ipynb) for interactive demos. ####
+Doctran converts messy, unstructured text ```    &#x004A; &#x0075; &#x006C;
+&#x0079; &#x0020; &#x0031; , &#x0032; &#x0030; &#x0032; &#x0033;   Updates and
+Discussions on Various Topics;
 Dear Team,
 I hope this email finds you well. In this document, I would like to provide you
 with some important updates and discuss various topics that require our
 attention. Please treat the information contained herein as highly
 confidential.
  Security and Privacy Measures
 As part of our ongoing commitment to ensure the security and privacy of our
@@ -32,18 +33,18 @@
 contributions to their respective departments. I would like to recognize Jane
 Smith (SSN: &#x0030; &#x0034; &#x0039; - &#x0034; &#x0035; - &#x0035; &#x0039;
 &#x0032; &#x0038;) for her outstanding performance in customer service. Jane
 has consistently received positive feedback from our clients. Furthermore,
 please remember that the open enrollment period for our employee benefits
 program is fast approaching. Should you have any questions or require
 assistance, please contact our HR representative, Michael Johnson (phone:
-&#x0034; &#x0031; ... ``` #### Into structured or semi-structured documents
-that are optimized for vector search. ``` { "topics": ["Security and Privacy",
-"HR Updates", "Marketing", "R&D"], "summary": "The document discusses updates
-on security measures, HR, marketing initiatives, and R&D projects. It commends
+&#x0034; &#x0031; ... ``` #### Into semi-structured documents that are
+optimized for vector search. ``` { "topics": ["Security and Privacy", "HR
+Updates", "Marketing", "R&D"], "summary": "The document discusses updates on
+security measures, HR, marketing initiatives, and R&D projects. It commends
 John Doe for enhancing network security, welcomes new team members, and
 recognizes Jane Smith for her customer service. It also mentions the open
 enrollment period for employee benefits, thanks Sarah Thompson for her social
 media efforts, and announces a product launch event on July 15th. David
 Rodriguez is acknowledged for his contributions to R&D. The document emphasizes
 the importance of confidentiality.", "contact_info": [ { "name": "John Doe",
 "contact_info": { "phone": "", "email": "john.doe@example.com" } }, { "name":
@@ -61,15 +62,15 @@
 Doctran is designed to make chaining document transformations easy. For
 example, you may want to first redact all PII from a document before sending it
 over to OpenAI to be summarized. Ordering is important when chaining
 transformations - transformations that are invoked first will be executed
 first, and its result will be passed to the next transformation. ```python
 document = await document.redact(entities=["EMAIL_ADDRESS",
 "PHONE_NUMBER"]).extract(properties).summarize().execute() ``` ##
-Doctransformers ### Extract Given any valid JSON schema, yses OpenAI function
+Doctransformers ### Extract Given any valid JSON schema, uses OpenAI function
 calling to extract structured data from a document. ```python from doctran
 import ExtractProperty properties = ExtractProperty
 ( name="millenial_or_boomer", description="A prediction of whether this
 document was written by a millenial or boomer", type="string", enum=
 ["millenial", "boomer"], required=True ) document = await document.extract
 (properties=properties).execute() ``` ### Redact Uses a spaCy model to remove
 names, emails, phone numbers and other sensitive information from a document.
```

### Comparing `doctran-0.0.2/doctran/doctran.py` & `doctran-0.0.3/doctran/doctran.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 from enum import Enum
 import spacy
 from presidio_analyzer import AnalyzerEngine
 from presidio_analyzer.nlp_engine import NlpEngineProvider
 from presidio_anonymizer import AnonymizerEngine
 from typing import List, Optional, Dict, Any, Literal
 from pydantic import BaseModel
-import requests
 
 class ExtractProperty(BaseModel):
     name: str
     description: str
     type: Literal["string", "number", "boolean", "array", "object"]
     items: Optional[List | Dict[str, Any]]
     enum: Optional[List[str]]
@@ -77,15 +76,15 @@
 class Document(BaseModel):
     uri: str
     id: str
     content_type: ContentType
     raw_content: str
     transformed_content: str
     config: DoctranConfig
-    extracted_properties: Optional[Dict[str, Any]] = {}
+    extracted_properties: Optional[Dict] = {}
     metadata: Optional[Dict[str, Any]] = None
 
     def properties_as_yaml(self) -> str:
         yaml_out = yaml.dump(self.extracted_properties, sort_keys=False)
         return yaml_out
 
     def extract(self, *, properties: List[ExtractProperty]) -> 'DocumentTransformationBuilder':
```

### Comparing `doctran-0.0.2/doctran/transformers/__pycache__/document_transformers.cpython-310.pyc` & `doctran-0.0.3/doctran/transformers/__pycache__/document_transformers.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `doctran-0.0.2/doctran/transformers/__pycache__/transformers.cpython-310.pyc` & `doctran-0.0.3/doctran/transformers/__pycache__/transformers.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `doctran-0.0.2/doctran/transformers/transformers.py` & `doctran-0.0.3/doctran/transformers/transformers.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 import spacy
 from presidio_analyzer import AnalyzerEngine
 from presidio_analyzer.nlp_engine import NlpEngineProvider
 from presidio_anonymizer import AnonymizerEngine
 from presidio_anonymizer.entities import OperatorConfig
 from typing import List, Optional, Dict, Any, Literal
 from pydantic import BaseModel
-import requests
 import tiktoken
 from doctran import Document, DoctranConfig, ExtractProperty, RecognizerEntity
 
 class TooManyTokensException(Exception):
     def __init__(self, content_token_size: int, token_limit: int):
         super().__init__(f"OpenAI document transformation failed. The document is {content_token_size} tokens long, which exceeds the token limit of {token_limit}.")
```

### Comparing `doctran-0.0.2/PKG-INFO` & `doctran-0.0.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,55 +1,50 @@
 Metadata-Version: 2.1
 Name: doctran
-Version: 0.0.2
+Version: 0.0.3
 Summary: Document transformation framework for vector based retrieval
 Author: Jason Fan
 Author-email: jason.wc.fan@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: bs4 (>=0.0.1,<0.0.2)
-Requires-Dist: jsonschema (>=4.17.3,<5.0.0)
 Requires-Dist: lxml (>=4.9.2,<5.0.0)
-Requires-Dist: mailbox (>=0.4,<0.5)
 Requires-Dist: openai (>=0.27.8,<0.28.0)
-Requires-Dist: pdfplumber (>=0.9.0,<0.10.0)
 Requires-Dist: presidio-analyzer (>=2.2.33,<3.0.0)
 Requires-Dist: presidio-anonymizer (>=2.2.33,<3.0.0)
 Requires-Dist: pydantic (>=1.10.9,<2.0.0)
-Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: spacy (>=3.5.4,<4.0.0)
 Requires-Dist: tiktoken (>=0.4.0,<0.5.0)
 Description-Content-Type: text/markdown
 
 <h2 align="center">
 🐛 Doctran
 </h2>
 
 <p align="center">
   <p align="center"><b>Doc</b>ument <b>tran</b>sformation framework to improve vector search results</p>
 </p>
 <p align="center">
-<a href="https://join.slack.com/t/psychicapi/shared_invite/zt-1ty1wz6w0-8jkmdvBpM5kj_Fh30EiCcg" target="_blank">
+<a href="https://join.slack.com/t/psychicapi/shared_invite/zt-1yptnhwcz-SiOCnrbqnBDsuzps9sEMSw" target="_blank">
     <img src="https://img.shields.io/badge/slack-join-blue.svg?logo=slack" alt="Slack">
 </a>
 </a>
 <a href="https://github.com/psychic-api/doctran/blob/main/LICENSE" target="_blank">
     <img src="https://img.shields.io/static/v1?label=license&message=MIT&color=blue" alt="License">
 </a>
 <a href="https://github.com/psychic-api/doctran/issues" target="_blank">
     <img src="https://img.shields.io/github/issues/psychic-api/doctran?color=blue" alt="Issues">
 </a>
   <a href="https://twitter.com/psychicapi" target="_blank">
     <img src="https://img.shields.io/twitter/follow/psychicapi?style=social" alt="Twitter">
 </a>
 </p>
 
-Vector databases are useful for retrieving context for LLMs, however they struggle to find relevant information if the source documents are indexed hapharzardly and information is sparse. Doctran uses LLMs and open source NLP libraries to transform raw text into clean, structured, information-dense documents that are optimized for vector space retrieval.
+Vector databases are useful for retrieving context for LLMs, however they struggle to find relevant information if the source documents are indexed hapharzardly and information is sparse. Doctran uses LLMs and open source NLP libraries to transform raw text into clean, structured, information-dense documents that are optimized for vector space retrieval. You can think of Doctran as a black box where messy strings go in and nice, clean, labelled strings come out.
 
 Doctran is maintained by [Psychic](https://github.com/psychic-api/psychic), the data integration layer for LLMs.
 
 ## Examples
 Clone or download [`examples.ipynb`](/examples.ipynb) for interactive demos.
 
 #### Doctran converts messy, unstructured text
@@ -68,15 +63,15 @@
 </section>
 <section>
 <header>HR Updates and Employee Benefits</header>
 <p>Recently, we welcomed several new team members who have made significant contributions to their respective departments. I would like to recognize Jane Smith (SSN: &#x0030; &#x0034; &#x0039; - &#x0034; &#x0035; - &#x0035; &#x0039; &#x0032; &#x0038;) for her outstanding performance in customer service. Jane has consistently received positive feedback from our clients. Furthermore, please remember that the open enrollment period for our employee benefits program is fast approaching. Should you have any questions or require assistance, please contact our HR representative, Michael Johnson (phone: &#x0034; &#x0031; 
 ...
 ```
 
-#### Into structured or semi-structured documents that are optimized for vector search.
+#### Into semi-structured documents that are optimized for vector search.
 
 ```
 {
   "topics": ["Security and Privacy", "HR Updates", "Marketing", "R&D"],
   "summary": "The document discusses updates on security measures, HR, marketing initiatives, and R&D projects. It commends John Doe for enhancing network security, welcomes new team members, and recognizes Jane Smith for her customer service. It also mentions the open enrollment period for employee benefits, thanks Sarah Thompson for her social media efforts, and announces a product launch event on July 15th. David Rodriguez is acknowledged for his contributions to R&D. The document emphasizes the importance of confidentiality.",
   "contact_info": [
     {
@@ -132,15 +127,15 @@
 ```python
 document = await document.redact(entities=["EMAIL_ADDRESS", "PHONE_NUMBER"]).extract(properties).summarize().execute()
 ```
 
 ## Doctransformers
 
 ### Extract
-Given any valid JSON schema, yses OpenAI function calling to extract structured data from a document.
+Given any valid JSON schema, uses OpenAI function calling to extract structured data from a document.
 
 ```python
 from doctran import ExtractProperty
 
 properties = ExtractProperty(
     name="millenial_or_boomer", 
     description="A prediction of whether this document was written by a millenial or boomer",
```

#### html2text {}

```diff
@@ -1,34 +1,33 @@
-Metadata-Version: 2.1 Name: doctran Version: 0.0.2 Summary: Document
+Metadata-Version: 2.1 Name: doctran Version: 0.0.3 Summary: Document
 transformation framework for vector based retrieval Author: Jason Fan Author-
 email: jason.wc.fan@gmail.com Requires-Python: >=3.10,<4.0 Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
-:: 3.10 Classifier: Programming Language :: Python :: 3.11 Requires-Dist: bs4
-(>=0.0.1,<0.0.2) Requires-Dist: jsonschema (>=4.17.3,<5.0.0) Requires-Dist:
-lxml (>=4.9.2,<5.0.0) Requires-Dist: mailbox (>=0.4,<0.5) Requires-Dist: openai
-(>=0.27.8,<0.28.0) Requires-Dist: pdfplumber (>=0.9.0,<0.10.0) Requires-Dist:
+:: 3.10 Classifier: Programming Language :: Python :: 3.11 Requires-Dist: lxml
+(>=4.9.2,<5.0.0) Requires-Dist: openai (>=0.27.8,<0.28.0) Requires-Dist:
 presidio-analyzer (>=2.2.33,<3.0.0) Requires-Dist: presidio-anonymizer
 (>=2.2.33,<3.0.0) Requires-Dist: pydantic (>=1.10.9,<2.0.0) Requires-Dist:
-requests (>=2.31.0,<3.0.0) Requires-Dist: spacy (>=3.5.4,<4.0.0) Requires-Dist:
-tiktoken (>=0.4.0,<0.5.0) Description-Content-Type: text/markdown
+spacy (>=3.5.4,<4.0.0) Requires-Dist: tiktoken (>=0.4.0,<0.5.0) Description-
+Content-Type: text/markdown
                            ***** ð Doctran *****
       Document transformation framework to improve vector search results
                                     [Slack]
  [License] [Issues] [Twitter]
 Vector databases are useful for retrieving context for LLMs, however they
 struggle to find relevant information if the source documents are indexed
 hapharzardly and information is sparse. Doctran uses LLMs and open source NLP
 libraries to transform raw text into clean, structured, information-dense
-documents that are optimized for vector space retrieval. Doctran is maintained
-by [Psychic](https://github.com/psychic-api/psychic), the data integration
-layer for LLMs. ## Examples Clone or download [`examples.ipynb`](/
-examples.ipynb) for interactive demos. #### Doctran converts messy,
-unstructured text ```    &#x004A; &#x0075; &#x006C; &#x0079; &#x0020; &#x0031;
-, &#x0032; &#x0030; &#x0032; &#x0033;   Updates and Discussions on Various
-Topics;
+documents that are optimized for vector space retrieval. You can think of
+Doctran as a black box where messy strings go in and nice, clean, labelled
+strings come out. Doctran is maintained by [Psychic](https://github.com/
+psychic-api/psychic), the data integration layer for LLMs. ## Examples Clone or
+download [`examples.ipynb`](/examples.ipynb) for interactive demos. ####
+Doctran converts messy, unstructured text ```    &#x004A; &#x0075; &#x006C;
+&#x0079; &#x0020; &#x0031; , &#x0032; &#x0030; &#x0032; &#x0033;   Updates and
+Discussions on Various Topics;
 Dear Team,
 I hope this email finds you well. In this document, I would like to provide you
 with some important updates and discuss various topics that require our
 attention. Please treat the information contained herein as highly
 confidential.
  Security and Privacy Measures
 As part of our ongoing commitment to ensure the security and privacy of our
@@ -44,18 +43,18 @@
 contributions to their respective departments. I would like to recognize Jane
 Smith (SSN: &#x0030; &#x0034; &#x0039; - &#x0034; &#x0035; - &#x0035; &#x0039;
 &#x0032; &#x0038;) for her outstanding performance in customer service. Jane
 has consistently received positive feedback from our clients. Furthermore,
 please remember that the open enrollment period for our employee benefits
 program is fast approaching. Should you have any questions or require
 assistance, please contact our HR representative, Michael Johnson (phone:
-&#x0034; &#x0031; ... ``` #### Into structured or semi-structured documents
-that are optimized for vector search. ``` { "topics": ["Security and Privacy",
-"HR Updates", "Marketing", "R&D"], "summary": "The document discusses updates
-on security measures, HR, marketing initiatives, and R&D projects. It commends
+&#x0034; &#x0031; ... ``` #### Into semi-structured documents that are
+optimized for vector search. ``` { "topics": ["Security and Privacy", "HR
+Updates", "Marketing", "R&D"], "summary": "The document discusses updates on
+security measures, HR, marketing initiatives, and R&D projects. It commends
 John Doe for enhancing network security, welcomes new team members, and
 recognizes Jane Smith for her customer service. It also mentions the open
 enrollment period for employee benefits, thanks Sarah Thompson for her social
 media efforts, and announces a product launch event on July 15th. David
 Rodriguez is acknowledged for his contributions to R&D. The document emphasizes
 the importance of confidentiality.", "contact_info": [ { "name": "John Doe",
 "contact_info": { "phone": "", "email": "john.doe@example.com" } }, { "name":
@@ -73,15 +72,15 @@
 Doctran is designed to make chaining document transformations easy. For
 example, you may want to first redact all PII from a document before sending it
 over to OpenAI to be summarized. Ordering is important when chaining
 transformations - transformations that are invoked first will be executed
 first, and its result will be passed to the next transformation. ```python
 document = await document.redact(entities=["EMAIL_ADDRESS",
 "PHONE_NUMBER"]).extract(properties).summarize().execute() ``` ##
-Doctransformers ### Extract Given any valid JSON schema, yses OpenAI function
+Doctransformers ### Extract Given any valid JSON schema, uses OpenAI function
 calling to extract structured data from a document. ```python from doctran
 import ExtractProperty properties = ExtractProperty
 ( name="millenial_or_boomer", description="A prediction of whether this
 document was written by a millenial or boomer", type="string", enum=
 ["millenial", "boomer"], required=True ) document = await document.extract
 (properties=properties).execute() ``` ### Redact Uses a spaCy model to remove
 names, emails, phone numbers and other sensitive information from a document.
```

