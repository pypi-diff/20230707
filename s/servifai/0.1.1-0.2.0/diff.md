# Comparing `tmp/servifai-0.1.1.tar.gz` & `tmp/servifai-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "servifai-0.1.1.tar", max compression
+gzip compressed data, was "servifai-0.2.0.tar", max compression
```

## Comparing `servifai-0.1.1.tar` & `servifai-0.2.0.tar`

### file list

```diff
@@ -1,16 +1,18 @@
--rw-r--r--   0        0        0     1067 2023-06-29 08:21:05.500102 servifai-0.1.1/LICENSE
--rw-r--r--   0        0        0     4372 2023-07-03 04:05:52.164398 servifai-0.1.1/README.md
--rw-r--r--   0        0        0      751 2023-07-03 04:14:35.980398 servifai-0.1.1/pyproject.toml
--rw-r--r--   0        0        0       53 2023-07-03 04:11:23.100398 servifai-0.1.1/servifai/__init__.py
--rw-r--r--   0        0        0      113 2023-06-30 05:42:21.396259 servifai-0.1.1/servifai/default_config.yaml
--rw-r--r--   0        0        0        0 2023-06-29 08:25:16.344102 servifai-0.1.1/servifai/llm/__init__.py
--rw-r--r--   0        0        0      849 2023-07-03 04:12:13.788398 servifai-0.1.1/servifai/llm/openai.py
--rw-r--r--   0        0        0        0 2023-06-29 08:25:16.344102 servifai-0.1.1/servifai/memory/__init__.py
--rw-r--r--   0        0        0     1467 2023-06-29 18:08:26.490413 servifai-0.1.1/servifai/memory/chroma.py
--rw-r--r--   0        0        0        0 2023-06-29 08:25:16.344102 servifai-0.1.1/servifai/planning/__init__.py
--rw-r--r--   0        0        0     1065 2023-07-03 03:50:52.248398 servifai-0.1.1/servifai/planning/react.py
--rw-r--r--   0        0        0     2437 2023-07-03 04:12:13.796398 servifai-0.1.1/servifai/servifai.py
--rw-r--r--   0        0        0        0 2023-06-29 08:25:16.344102 servifai-0.1.1/servifai/toolbox/__init__.py
--rw-r--r--   0        0        0     1291 2023-06-30 06:16:35.092259 servifai-0.1.1/servifai/toolbox/default.py
--rw-r--r--   0        0        0     6689 2023-07-03 03:50:40.432398 servifai-0.1.1/servifai/toolbox/knowledge_base.py
--rw-r--r--   0        0        0     5292 1970-01-01 00:00:00.000000 servifai-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-06-29 08:21:05.500102 servifai-0.2.0/LICENSE
+-rw-r--r--   0        0        0     4273 2023-07-07 16:02:37.891863 servifai-0.2.0/README.md
+-rw-r--r--   0        0        0      773 2023-07-07 16:03:13.607863 servifai-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0       53 2023-07-07 16:03:00.447863 servifai-0.2.0/servifai/__init__.py
+-rw-r--r--   0        0        0      243 2023-07-07 16:02:37.899863 servifai-0.2.0/servifai/default_config.yaml
+-rw-r--r--   0        0        0       26 2023-07-07 16:02:37.899863 servifai-0.2.0/servifai/llm/__init__.py
+-rw-r--r--   0        0        0      389 2023-07-07 16:02:37.899863 servifai-0.2.0/servifai/llm/base.py
+-rw-r--r--   0        0        0     1343 2023-07-07 16:02:37.899863 servifai-0.2.0/servifai/llm/openai.py
+-rw-r--r--   0        0        0       29 2023-07-07 16:02:37.899863 servifai-0.2.0/servifai/memory/__init__.py
+-rw-r--r--   0        0        0     1780 2023-07-07 16:02:37.899863 servifai-0.2.0/servifai/memory/chroma.py
+-rw-r--r--   0        0        0       34 2023-07-07 16:02:37.899863 servifai-0.2.0/servifai/planning/__init__.py
+-rw-r--r--   0        0        0      891 2023-07-07 16:02:37.899863 servifai-0.2.0/servifai/planning/react.py
+-rw-r--r--   0        0        0     2090 2023-07-07 16:02:37.899863 servifai-0.2.0/servifai/servifai.py
+-rw-r--r--   0        0        0       30 2023-07-07 16:02:37.899863 servifai-0.2.0/servifai/toolbox/__init__.py
+-rw-r--r--   0        0        0      864 2023-07-07 16:02:37.899863 servifai-0.2.0/servifai/toolbox/base.py
+-rw-r--r--   0        0        0     1285 2023-07-07 16:02:37.899863 servifai-0.2.0/servifai/toolbox/default.py
+-rw-r--r--   0        0        0     6645 2023-07-07 16:02:37.899863 servifai-0.2.0/servifai/toolbox/knowledge_base.py
+-rw-r--r--   0        0        0     5193 1970-01-01 00:00:00.000000 servifai-0.2.0/PKG-INFO
```

### Comparing `servifai-0.1.1/LICENSE` & `servifai-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `servifai-0.1.1/README.md` & `servifai-0.2.0/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -9,21 +9,22 @@
 
 **ServifAI (Task-based Agent) = LLM + Memory + Planning + Toolbox**
 
 ![agent_pic](https://lilianweng.github.io/posts/2023-06-23-agent/agent-overview.png)
 
 Instead of feeding all kinds of tools to a single agent and confusing it while selection, **ServifAI** narrows down the selection by combining only necessary tools on basis of the task at hand.
 
-Read [this article to understand How Agents works](https://lilianweng.github.io/posts/2023-06-23-agent/). 
+Read [this article to get an overview on Agents](https://lilianweng.github.io/posts/2023-06-23-agent/). 
 
-By default, **ServifAI** can chat while browsing internet and solving common math problems.
+### Current Supported Tasks:
+|  Tasks | Toolbox Tools |
+| :------ | :---------------: |
+| `default` | DuckDuckGo + LLM Math + PAL Math |
+| `qna_local_docs` | Vector Index + Knowledge Graphs |
 
-### Current Toolbox Status:
-- Default (DuckDuckgo + LLM Math + PAL Math)
-- QA Knowledge Base (Vector Index + Knowledge Graphs)
 
 ## Installation
 Works best with [Poetry](https://python-poetry.org/docs/)
 ```bash
 poetry add servifai
 ```
 With pip, you might have to install dependencies manually
@@ -40,77 +41,80 @@
 Run Python Code
 ```python
 from servifai import ServifAI
 myagent = ServifAI()
 
 while True:
     text_input = input("Me: ")
-    response = myagent.query(text_input)
+    if text_input == "exit":
+        break
+    response = myagent.chat(text_input)
     print(f'ServifAI: {response}\n')
 ```
 Output
 ```
 Me: Hi, How are you?
 ServifAI: Hi, I'm an AI language model, so I don't have feelings, but I'm here to help you with any questions or tasks you have!
 
 Me: What is the current weather of Bengaluru?
 ServifAI: The current weather in Bengaluru is mostly cloudy with a temperature of 81°F (27°C). The wind is coming from the north at 3 mph (5 km/h). Tomorrow's temperature is expected to be nearly the same as today.
 
 ```
 ## Data Creation Recipe for Local Knowledge Extraction Tasks
 Consider the example of [Uber 10Q filings](https://investor.uber.com/financials/default.aspx). 
 - Download the quaterly reports for year 2022 and 2023 as pdf and save it locally in a directory (here `reports`).
-- Create a config YAML file `uber_10q.yaml` inside a `configs` dir and fill details as:
+- Create a config YAML file `uber10q.yaml` inside a `configs` dir and fill details as:
 ```yaml
-task: 'qa_knowledge_base'
+task: qna_local_docs
 
-vectordb:
-  dir: "uber_10q"
+llm:
+  org: openai
+  model: gpt-3.5-turbo
+  temperature: 0
+  max_tokens: 3000
 
 data:
-  dir: "reports"
+  dir: reports
   about: "Uber 10Q Filing"
 
-text:
+memory:
+  dir: uber_10q
   max_input_size: 2500
   num_outputs: 1000
   max_chunk_overlap: 0.05
   chunk_size_limit: 1000
-
-llm:
-  org: openai
-  temperature: 0
-  model_name: "gpt-3.5-turbo"
 ```
-- As the task is to extract information from these pdfs, so task chosen is `qa_knowledge_base`. Based on these tasks we choose our *toolbox* which contains specific tools required for task completion. We will be adding more *toolbox*.
+- As the task is to extract information from these pdfs, so task chosen is `qna_local_docs`. Based on these tasks ServifAI chooses *toolbox* which contains specific tools required for task completion. We will be adding more *toolbox* later.
 - To achieve optimum results, its recommended to rename your pdfs as *few words description*. For example, we rename quarterly 10Q reports as `Q1-23.pdf`, `Q4-22.pdf` etc. Do not add blank spaces between words, instead use `hyphen -`. 
 - Also in config file in `data.about`, provide a concise common summary of all these multiple pdfs. For example, here we write this as `Uber 10Q Filing`.
 - Run Python Code
 ```python
 from servifai import ServifAI
-myagent = ServifAI('configs/uber_10q.yaml')
+myagent = ServifAI('configs/uber10q.yaml')
 
 while True:
     text_input = input("Me: ")
-    response = myagent.query(text_input)
+    if text_input == "exit":
+        break
+    response = myagent.chat(text_input)
     print(f'ServifAI: {response}\n')
 ```
 - Output
 ```
-Me: Analyze the revenue growth of Uber across quarters
-ServifAI: Based on the provided context information, the revenue growth of Uber across quarters can be summarized as follows:
+Me: Analyze the revenue growth of Uber across last few quarters
+ServifAI: Based on the provided context, Uber's revenue growth in the last few quarters can be summarized as follows:
 
-- Q3 2022: Revenue growth of 72% year-over-year or 81% on a constant currency basis.
-- Q4 2022: Revenue growth of 59% on a constant currency basis, significantly outpacing the 19% growth in Gross Bookings.
-- Q1 2023: Revenue of $8.8 billion is mentioned, but the growth rate for this quarter is not provided.
+- Q3 2022: 72% year-over-year or 81% on a constant currency basis.
+- Q4 2022: 49% year-over-year.
+- Q1 2023: 29% year-over-year or 33% on a constant currency basis.
 
-Therefore, the specific revenue growth rate for Q1 2023 cannot be determined with the given information.
+Therefore, Uber's revenue growth in the last few quarters has been positive, with varying rates of growth.
 
 Me: How much cash did Uber have in last quarter of 2022?
-ServifAI: Based on the provided context, the cash balance for Uber at the end of Q4 2022 was $4.3 billion.
+ServifAI: Based on the provided context, the cash balance for Uber in Q4 2022 was $4.3 billion.
 
 ```
 
 # TODO:
 - [ ] Add other task based tools
 - [ ] Add support for Local LLMs
 - [ ] Add support for other VectorDBs
```

### Comparing `servifai-0.1.1/pyproject.toml` & `servifai-0.2.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "servifai"
-version = "0.1.1"
+version = "0.2.0"
 description = "A mini framework built on top of Langchain and Llamaindex to provide LLM powered Autonomous Agents as a simplified service to assist users with their tasks"
 authors = ["Zoheb Abai <zohebabai@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
@@ -18,11 +18,12 @@
 nltk = "^3.8.1"
 duckduckgo-search = "^3.8.3"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.4.0"
 pre-commit = "^3.3.3"
 scriv = {extras = ["toml"], version = "^1.3.1"}
+jupyterlab = "^4.0.2"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `servifai-0.1.1/servifai/memory/chroma.py` & `servifai-0.2.0/servifai/memory/chroma.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,43 +1,53 @@
 import os
+
 import chromadb
 from chromadb.config import Settings
-from chromadb.utils import embedding_functions
 from dotenv import load_dotenv
+from langchain.embeddings import OpenAIEmbeddings
+from llama_index import LangchainEmbedding
+
 load_dotenv()
 
 
 class ChromaDB:
-    def __init__(self, db_dir, oai_org=None):
+    def __init__(self, db_dir):
         self._path = db_dir
-        self._oai_org = oai_org
-        self._embed = self._get_openai_embeddings()
+        self._oai_org = os.getenv("OPENAI_API_TYPE")
         self._client_settings = chromadb.config.Settings(
             chroma_db_impl="duckdb+parquet",
             persist_directory=str(self._path),
             anonymized_telemetry=False,
         )
+        self.embed = self._get_openai_embeddings()
         self.client = self._get_or_create_db()
         self.collection = self._get_or_create_collection()
 
     def _get_openai_embeddings(self):
-        if 'azure' in self._oai_org:
-            return embedding_functions.OpenAIEmbeddingFunction(
-                api_key=os.getenv("OPENAI_API_KEY"),
-                api_base=os.getenv("API_BASE_PATH"),
-                api_type="azure",
-                model_name="text-embedding-ada-002"
+        if self._oai_org == "azure":
+            return LangchainEmbedding(
+                OpenAIEmbeddings(
+                    model="text-embedding-ada-002",
+                    deployment="text-embedding-ada-002",
+                    openai_api_type="azure",
+                    openai_api_key=os.getenv("OPENAI_API_KEY"),
+                    openai_api_base=os.getenv("OPENAI_API_BASE"),
+                    openai_api_version=os.getenv("OPENAI_API_VERSION"),
+                ),
+                embed_batch_size=1,
             )
-        return embedding_functions.OpenAIEmbeddingFunction(
-            api_key=os.getenv("OPENAI_API_KEY"),
-            model_name="text-embedding-ada-002"
+        return LangchainEmbedding(
+            OpenAIEmbeddings(
+                model="text-embedding-ada-002",
+                openai_api_key=os.getenv("OPENAI_API_KEY"),
+            ),
         )
 
     def _get_or_create_db(self):
         return chromadb.Client(self._client_settings)
 
     def _get_or_create_collection(self):
         return self.client.get_or_create_collection(
             name=self._path.stem,
             metadata={"hnsw:space": "cosine"},
-            embedding_function=self._embed,
-        )
+            embedding_function=self.embed,
+        )
```

### Comparing `servifai-0.1.1/servifai/servifai.py` & `servifai-0.2.0/servifai/servifai.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 # Import Libraries
 import logging
 import sys
 from pathlib import Path
 
 import yaml
 
-from servifai.llm.openai import OpenAILLM
-from servifai.planning.react import ReactChatAgent
-from servifai.toolbox.knowledge_base import KnowledgeBase
+from servifai.llm import BaseLLM
+from servifai.planning import ReactChatAgent
 
 logging.basicConfig(stream=sys.stdout, level=logging.INFO)
 logging.getLogger().addHandler(logging.StreamHandler(stream=sys.stdout))
 
 BASE_DIR = Path(__file__).parent.parent.absolute()
 LOGS_DIR = Path(BASE_DIR, "logs")
 DEFAULT_CONFIG = Path(BASE_DIR, "servifai/default_config.yaml")
@@ -22,53 +21,47 @@
         """Initializes a ServifAI instance with specific config for a given task
 
         Args:
             cfg (DictConfig): specific constants for a particular data
         """
         self.cfg = self._load_config(config_file)
         self.task = self.cfg["task"]
-        self.oaillm = OpenAILLM(
-            self.cfg["llm"], self.cfg["text"]
-        )  # if 'openai' in self.cfg['llm']['org'] else None
-        self.knowledgebase = (
-            KnowledgeBase(
-                Path(BASE_DIR, self.cfg["vectordb"]["dir"]),
-                Path(BASE_DIR, self.cfg["data"]["dir"]),
-                self.cfg["data"]["about"],
-                self.cfg["text"],
-                self.cfg["llm"],
-            )
-            if self.task == "qa_knowledge_base"
-            else None
+        self.llm = BaseLLM(self.cfg["llm"]).llm
+        self.agent = ReactChatAgent(
+            self.task,
+            self.llm,
+            Path(BASE_DIR, self.cfg["memory"]["dir"]),
+            Path(BASE_DIR, self.cfg["data"]["dir"]),
+            self.cfg["data"],
+            self.cfg["memory"],
         )
-        self.agent = ReactChatAgent(self.task, self.knowledgebase, self.oaillm)
 
     def _load_config(self, config_file):
         config = None
         if config_file is not None and Path(config_file).exists():
             with open(config_file, "r") as file:
                 config = yaml.safe_load(file)
         else:
             logging.warning(
                 "No Config file provided by user, hence switching to default!"
             )
             with open(DEFAULT_CONFIG, "r") as file:
                 config = yaml.safe_load(file)
         return config
 
-    def query(self, question: str):
+    def chat(self, question: str):
         """Responds to user query as chat conversation
 
         Args:
             question (str): user query
 
         Returns:
             str: Response
         """
         try:
-            if question != "":
-                logging.info("Generating response:")
-                return self.agent.chat(question)
-            else:
+            if not question:
                 logging.warning("No input text provided by user")
+                return "No input provided by user"
+            logging.info("Generating response:")
+            return self.agent.query(question)
         except Exception as e:
-            logging.error(f"Error {e} occured")
+            logging.error(f"Error: {e}")
```

### Comparing `servifai-0.1.1/servifai/toolbox/default.py` & `servifai-0.2.0/servifai/toolbox/default.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from langchain.agents import Tool
 from langchain.chains import LLMMathChain, PALChain
 from langchain.tools import DuckDuckGoSearchRun
 
 
 class DefaultTools:
     def __init__(self, llm):
-        self.llm = llm.model
+        self.llm = llm
         self.palmath_tool = self._get_pal_math()
         self.llmmath_tool = self._get_llm_math()
         self.web_search = self._get_ddg_search()
 
     def _get_pal_math(self):
         return Tool(
             name="PAL-MATH",
```

### Comparing `servifai-0.1.1/servifai/toolbox/knowledge_base.py` & `servifai-0.2.0/servifai/toolbox/knowledge_base.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,16 +11,15 @@
 )
 from llama_index.indices.composability import ComposableGraph
 from llama_index.indices.keyword_table import SimpleKeywordTableIndex
 from llama_index.indices.query.query_transform.base import DecomposeQueryTransform
 from llama_index.query_engine.transform_query_engine import TransformQueryEngine
 from llama_index.vector_stores import ChromaVectorStore
 
-from servifai.llm.openai import OpenAILLM
-from servifai.memory.chroma import ChromaDB
+from servifai.memory import ChromaDB
 
 
 class VectorKnowledgeBase:
     def __init__(self, vector_indices, index_summaries, service_context):
         self._indices = vector_indices
         self._summaries = index_summaries
         self._service_context = service_context
@@ -30,15 +29,15 @@
         summary = self._summaries[title]
         query_engine = index.as_query_engine(
             service_context=self._service_context, similarity_top_k=3
         )
         return Tool(
             name=f"Knowledge Vector Index {title}",
             func=lambda q: str(query_engine.query(q)),
-            description=f"useful for when you want to answer queries just on {summary}",
+            description=f"useful for answering queries only regarding {summary}",
             return_direct=True,
         )
 
 
 class KnowledgeGraphs:
     def __init__(self, vector_indices, index_summaries, service_context, llm_predictor):
         self._indices = vector_indices
@@ -79,52 +78,52 @@
             custom_query_engines=self._custom_query_engines
         )
 
     def as_tool(self, about):
         return Tool(
             name="Knowledge Graph Index",
             func=lambda q: str(self._query_engine.query(q)),
-            description=f"useful for when you want to answer queries that require comparing/contrasting or analyzing over multiple sources of {about}",
+            description=f"useful for answering queries that require comparing/contrasting or analyzing over multiple sources about {about}",
             return_direct=True,
         )
 
 
 class KnowledgeBase:
-    def __init__(self, vdb_dir, data_dir, about, text, llm):
+    def __init__(self, vdb_dir, data_dir, about, memoryconfigs, oaillm):
         self.vdb_dir = vdb_dir
         self.data_dir = data_dir
         self.about = about
-        self.max_input_size = int(text["max_input_size"])
-        self.num_outputs = int(text["num_outputs"])
-        self.max_chunk_overlap = float(text["max_chunk_overlap"])
-        self.chunk_size_limit = int(text["chunk_size_limit"])
-        self.llm = llm
-        self.oaillm = OpenAILLM(llm, text)
-        self.llm_predictor = LLMPredictor(llm=self.oaillm.model)
+        self.max_input_size = int(memoryconfigs["max_input_size"])
+        self.num_outputs = int(memoryconfigs["num_outputs"])
+        self.max_chunk_overlap = float(memoryconfigs["max_chunk_overlap"])
+        self.chunk_size_limit = int(memoryconfigs["chunk_size_limit"])
+        self.llm_predictor = LLMPredictor(llm=oaillm.model)
+        self.vectordb = ChromaDB(self.vdb_dir)
         self.vectorstore = self._initiate_vectorstore()
         self.service_context = self._initiate_contexts()[0]
         self.storage_context = self._initiate_contexts()[1]
         self.titles = []
         self.indices = self._create_indices()[0]
         self.index_summaries = self._create_indices()[1]
         self.qe_tools = self._get_query_engine_tools()
 
     def _initiate_vectorstore(self):
-        vectordb = ChromaDB(self.vdb_dir, self.llm["org"])
-        return ChromaVectorStore(chroma_collection=vectordb.collection)
+        return ChromaVectorStore(chroma_collection=self.vectordb.collection)
 
     def _initiate_contexts(self):
         prompt_helper = PromptHelper(
             self.max_input_size,
             self.num_outputs,
             self.max_chunk_overlap,
             chunk_size_limit=self.chunk_size_limit,
         )
         self.service_context = ServiceContext.from_defaults(
-            llm_predictor=self.llm_predictor, prompt_helper=prompt_helper
+            llm_predictor=self.llm_predictor,
+            prompt_helper=prompt_helper,
+            embed_model=self.vectordb.embed,
         )
         self.storage_context = StorageContext.from_defaults(
             vector_store=self.vectorstore
         )
         return self.service_context, self.storage_context
 
     def _create_indices(self):
@@ -137,31 +136,30 @@
         """
         ext = ".pdf"
         docs = {}
         indices = {}
         index_summaries = {}
 
         for dbb in Path(self.data_dir).glob(f"*{ext}"):
-            print(dbb)
-            title = dbb.stem
+            title = " ".join(dbb.stem.split("-"))
             self.titles.append(title)
             docs[title] = SimpleDirectoryReader(
                 input_files=[str(dbb)],
                 recursive=True,
                 exclude_hidden=True,
                 required_exts=[ext],
             ).load_data()
             indices[title] = VectorStoreIndex.from_documents(
                 docs[title],
                 service_context=self.service_context,
                 storage_context=self.storage_context,
             )
             index_summaries[
                 title
-            ] = f"individual source on {self.about} for particular {' '.join(title.split('-'))}"
+            ] = f"individual source generally about {self.about} and particularly on {title}"
         return indices, index_summaries
 
     def _get_query_engine_tools(self):
         qe_tools = []
         for title in self.titles:
             vectorkb_tool = VectorKnowledgeBase(
                 self.indices, self.index_summaries, self.service_context
```

### Comparing `servifai-0.1.1/PKG-INFO` & `servifai-0.2.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: servifai
-Version: 0.1.1
+Version: 0.2.0
 Summary: A mini framework built on top of Langchain and Llamaindex to provide LLM powered Autonomous Agents as a simplified service to assist users with their tasks
 License: MIT
 Author: Zoheb Abai
 Author-email: zohebabai@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -32,21 +32,22 @@
 
 **ServifAI (Task-based Agent) = LLM + Memory + Planning + Toolbox**
 
 ![agent_pic](https://lilianweng.github.io/posts/2023-06-23-agent/agent-overview.png)
 
 Instead of feeding all kinds of tools to a single agent and confusing it while selection, **ServifAI** narrows down the selection by combining only necessary tools on basis of the task at hand.
 
-Read [this article to understand How Agents works](https://lilianweng.github.io/posts/2023-06-23-agent/). 
+Read [this article to get an overview on Agents](https://lilianweng.github.io/posts/2023-06-23-agent/). 
 
-By default, **ServifAI** can chat while browsing internet and solving common math problems.
+### Current Supported Tasks:
+|  Tasks | Toolbox Tools |
+| :------ | :---------------: |
+| `default` | DuckDuckGo + LLM Math + PAL Math |
+| `qna_local_docs` | Vector Index + Knowledge Graphs |
 
-### Current Toolbox Status:
-- Default (DuckDuckgo + LLM Math + PAL Math)
-- QA Knowledge Base (Vector Index + Knowledge Graphs)
 
 ## Installation
 Works best with [Poetry](https://python-poetry.org/docs/)
 ```bash
 poetry add servifai
 ```
 With pip, you might have to install dependencies manually
@@ -63,77 +64,80 @@
 Run Python Code
 ```python
 from servifai import ServifAI
 myagent = ServifAI()
 
 while True:
     text_input = input("Me: ")
-    response = myagent.query(text_input)
+    if text_input == "exit":
+        break
+    response = myagent.chat(text_input)
     print(f'ServifAI: {response}\n')
 ```
 Output
 ```
 Me: Hi, How are you?
 ServifAI: Hi, I'm an AI language model, so I don't have feelings, but I'm here to help you with any questions or tasks you have!
 
 Me: What is the current weather of Bengaluru?
 ServifAI: The current weather in Bengaluru is mostly cloudy with a temperature of 81°F (27°C). The wind is coming from the north at 3 mph (5 km/h). Tomorrow's temperature is expected to be nearly the same as today.
 
 ```
 ## Data Creation Recipe for Local Knowledge Extraction Tasks
 Consider the example of [Uber 10Q filings](https://investor.uber.com/financials/default.aspx). 
 - Download the quaterly reports for year 2022 and 2023 as pdf and save it locally in a directory (here `reports`).
-- Create a config YAML file `uber_10q.yaml` inside a `configs` dir and fill details as:
+- Create a config YAML file `uber10q.yaml` inside a `configs` dir and fill details as:
 ```yaml
-task: 'qa_knowledge_base'
+task: qna_local_docs
 
-vectordb:
-  dir: "uber_10q"
+llm:
+  org: openai
+  model: gpt-3.5-turbo
+  temperature: 0
+  max_tokens: 3000
 
 data:
-  dir: "reports"
+  dir: reports
   about: "Uber 10Q Filing"
 
-text:
+memory:
+  dir: uber_10q
   max_input_size: 2500
   num_outputs: 1000
   max_chunk_overlap: 0.05
   chunk_size_limit: 1000
-
-llm:
-  org: openai
-  temperature: 0
-  model_name: "gpt-3.5-turbo"
 ```
-- As the task is to extract information from these pdfs, so task chosen is `qa_knowledge_base`. Based on these tasks we choose our *toolbox* which contains specific tools required for task completion. We will be adding more *toolbox*.
+- As the task is to extract information from these pdfs, so task chosen is `qna_local_docs`. Based on these tasks ServifAI chooses *toolbox* which contains specific tools required for task completion. We will be adding more *toolbox* later.
 - To achieve optimum results, its recommended to rename your pdfs as *few words description*. For example, we rename quarterly 10Q reports as `Q1-23.pdf`, `Q4-22.pdf` etc. Do not add blank spaces between words, instead use `hyphen -`. 
 - Also in config file in `data.about`, provide a concise common summary of all these multiple pdfs. For example, here we write this as `Uber 10Q Filing`.
 - Run Python Code
 ```python
 from servifai import ServifAI
-myagent = ServifAI('configs/uber_10q.yaml')
+myagent = ServifAI('configs/uber10q.yaml')
 
 while True:
     text_input = input("Me: ")
-    response = myagent.query(text_input)
+    if text_input == "exit":
+        break
+    response = myagent.chat(text_input)
     print(f'ServifAI: {response}\n')
 ```
 - Output
 ```
-Me: Analyze the revenue growth of Uber across quarters
-ServifAI: Based on the provided context information, the revenue growth of Uber across quarters can be summarized as follows:
+Me: Analyze the revenue growth of Uber across last few quarters
+ServifAI: Based on the provided context, Uber's revenue growth in the last few quarters can be summarized as follows:
 
-- Q3 2022: Revenue growth of 72% year-over-year or 81% on a constant currency basis.
-- Q4 2022: Revenue growth of 59% on a constant currency basis, significantly outpacing the 19% growth in Gross Bookings.
-- Q1 2023: Revenue of $8.8 billion is mentioned, but the growth rate for this quarter is not provided.
+- Q3 2022: 72% year-over-year or 81% on a constant currency basis.
+- Q4 2022: 49% year-over-year.
+- Q1 2023: 29% year-over-year or 33% on a constant currency basis.
 
-Therefore, the specific revenue growth rate for Q1 2023 cannot be determined with the given information.
+Therefore, Uber's revenue growth in the last few quarters has been positive, with varying rates of growth.
 
 Me: How much cash did Uber have in last quarter of 2022?
-ServifAI: Based on the provided context, the cash balance for Uber at the end of Q4 2022 was $4.3 billion.
+ServifAI: Based on the provided context, the cash balance for Uber in Q4 2022 was $4.3 billion.
 
 ```
 
 # TODO:
 - [ ] Add other task based tools
 - [ ] Add support for Local LLMs
 - [ ] Add support for other VectorDBs
```

