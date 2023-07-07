# Comparing `tmp/h2o_helium-0.4.0-py3-none-any.whl.zip` & `tmp/h2o_helium-0.5.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 4622 bytes, number of entries: 5
--rw-rw-r--  2.0 unx    12842 b- defN 23-Jun-13 10:33 h2o_helium/__init__.py
--rw-rw-r--  2.0 unx     1997 b- defN 23-Jun-13 10:33 h2o_helium-0.4.0.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jun-13 10:33 h2o_helium-0.4.0.dist-info/WHEEL
--rw-rw-r--  2.0 unx       11 b- defN 23-Jun-13 10:33 h2o_helium-0.4.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      390 b- defN 23-Jun-13 10:33 h2o_helium-0.4.0.dist-info/RECORD
-5 files, 15332 bytes uncompressed, 3896 bytes compressed:  74.6%
+Zip file size: 4762 bytes, number of entries: 5
+-rw-rw-r--  2.0 unx    13011 b- defN 23-Jul-07 10:05 h2o_helium/__init__.py
+-rw-rw-r--  2.0 unx     2014 b- defN 23-Jul-07 10:05 h2o_helium-0.5.0.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jul-07 10:05 h2o_helium-0.5.0.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       11 b- defN 23-Jul-07 10:05 h2o_helium-0.5.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      390 b- defN 23-Jul-07 10:05 h2o_helium-0.5.0.dist-info/RECORD
+5 files, 15518 bytes uncompressed, 4036 bytes compressed:  74.0%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
 Filename: h2o_helium/__init__.py
 Comment: 
 
-Filename: h2o_helium-0.4.0.dist-info/METADATA
+Filename: h2o_helium-0.5.0.dist-info/METADATA
 Comment: 
 
-Filename: h2o_helium-0.4.0.dist-info/WHEEL
+Filename: h2o_helium-0.5.0.dist-info/WHEEL
 Comment: 
 
-Filename: h2o_helium-0.4.0.dist-info/top_level.txt
+Filename: h2o_helium-0.5.0.dist-info/top_level.txt
 Comment: 
 
-Filename: h2o_helium-0.4.0.dist-info/RECORD
+Filename: h2o_helium-0.5.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## h2o_helium/__init__.py

```diff
@@ -6,15 +6,15 @@
 from typing import Iterable, Optional, List
 from urllib.parse import urlparse
 
 import requests
 from pydantic import BaseModel
 from websockets.sync.client import connect as ws_connect, ClientConnection
 
-__version__ = '0.4.0'
+__version__ = '0.5.0'
 
 
 class Status(str, Enum):
     Unknown = 'unknown'
     Scheduled = 'scheduled'
     Queued = 'queued'
     Running = 'running'
@@ -26,14 +26,21 @@
 class ChatMessage(BaseModel):
     id: str
     content: str
     reply_to: Optional[str]
     created_at: datetime
 
 
+class ChatMessageReference(BaseModel):
+    document_id: str
+    document_name: str
+    chunk_id: int
+    score: float
+
+
 class ChatSessionCount(BaseModel):
     chat_session_count: int
 
 
 class ChatSessionForCollection(BaseModel):
     id: str
     latest_message_content: Optional[str]
@@ -45,17 +52,19 @@
     latest_message_content: Optional[str]
     collection_id: str
     collection_name: str
     updated_at: datetime
 
 
 class Chunk(BaseModel):
-    id: str
-    content: str
-    position: int
+    text: str
+
+
+class Chunks(BaseModel):
+    chunks: List[Chunk]
 
 
 class Collection(BaseModel):
     id: str
     name: str
     description: str
     document_count: int
@@ -162,15 +171,15 @@
         self._connection: Optional[ClientConnection] = None
 
     def connect(self):
         self._connection = ws_connect(self._address, additional_headers={
             'Authorization': f'Bearer {self._api_key}'
         })
 
-    def query(self, message: str, timeout: Optional[float] = None) -> str:
+    def query(self, message: str, timeout: Optional[float] = None) -> ChatMessage:
         correlation_id = str(uuid.uuid4())
         req = dict(
             s=self._chat_session_id,
             x=correlation_id,
             b=message,
         )
         self._connection.send(marshal(req))
@@ -181,29 +190,35 @@
         while True:
             res = self._connection.recv(deadline - time.time())
 
             data = unmarshal(res)
             t = data['t']
             chat_session_id = data['s']
             reply_to_id = data['x']
+            message_id = data.get('a', None)
             body = data['b']
 
             if chat_session_id != self._chat_session_id:
                 continue
 
             if t == 'a':  # ack
                 if reply_to_id == correlation_id:
                     request_id = body
             elif t == 'p':
                 if reply_to_id == request_id:
                     response += body
             elif t == 'f':
                 if reply_to_id == request_id:
                     response += body
-                    return response
+                    return ChatMessage(
+                        id=message_id,
+                        content=response,
+                        reply_to=reply_to_id,
+                        created_at=datetime.now(),
+                    )
             elif t == 'e':
                 if reply_to_id == request_id:
                     raise SessionError(f'Remote error: {body}')
             else:
                 raise SessionError(f'Invalid chat response type {t}.')
 
     def disconnect(self):
@@ -250,14 +265,17 @@
 
     def _db(self, method: str, *args):
         return self._post('/rpc/db', marshal([method, *args]))
 
     def _job(self, method: str, **kwargs):
         return self._post('/rpc/job', marshal([method, kwargs]))
 
+    def _vex(self, method: str, **kwargs):
+        return self._post('/rpc/vex', marshal(dict(method=method, params=kwargs)))
+
     def _wait(self, d):
         job_id = _to_id(d)
         while True:
             time.sleep(1)
             job = self.get_job(job_id)
             if job.completed or job.canceled:
                 break
@@ -299,19 +317,18 @@
     def delete_documents(self, document_ids: Iterable[str]):
         return self._wait(self._job('crawl.DeleteDocumentsJob', document_ids=document_ids))
 
     def delete_documents_from_collection(self, collection_id: str, document_ids: Iterable[str]):
         return self._wait(self._job('crawl.DeleteDocumentsFromCollectionJob', collection_id=collection_id,
                                     document_ids=document_ids))
 
-    def get_chunk(self, document_id: str, chunk_id: str) -> Chunk:
-        res = self._db('get_chunk', document_id, chunk_id)
-        if len(res) == 0:
-            raise KeyError(f'Chunk {chunk_id} not found')
-        return Chunk(**res[0])
+    def get_chunks(self, collection_id: str, chunk_ids: Iterable[int]) -> List[Chunk]:
+        res = self._vex('get_chunks', collection_id=collection_id, chunk_ids=list(chunk_ids))
+        chunks = Chunks(**res).chunks
+        return chunks
 
     def get_collection(self, collection_id: str) -> Collection:
         res = self._db('get_collection', collection_id)
         if len(res) == 0:
             raise KeyError(f'Collection {collection_id} not found')
         return Collection(**res[0])
 
@@ -346,28 +363,23 @@
 
     def ingest_website(self, collection_id: str, url: str):
         return self._wait(self._job('crawl.IngestWebsiteJob', collection_id=collection_id, url=url))
 
     def list_chat_messages(self, chat_session_id: str, offset: int, limit: int) -> List[ChatMessage]:
         return [ChatMessage(**d) for d in self._db('list_chat_messages', chat_session_id, offset, limit)]
 
-    def list_chat_sessions_for_collection(self, collection_id: str, offset: int, limit: int) -> List[
-        ChatSessionForCollection]:
+    def list_chat_message_references(self, message_id: str) -> List[ChatMessageReference]:
+        return [ChatMessageReference(**d) for d in self._db('list_chat_message_references', message_id)]
+
+    def list_chat_sessions_for_collection(
+            self, collection_id: str, offset: int, limit: int
+    ) -> List[ChatSessionForCollection]:
         return [ChatSessionForCollection(**d) for d in
                 self._db('list_chat_sessions_for_collection', collection_id, offset, limit)]
 
-    def list_chunks(self, document_id: str, offset: int, limit: int) -> List[Chunk]:
-        return [Chunk(**d) for d in self._db('list_chunks', document_id, offset, limit)]
-
-    def list_chunks_after(self, document_id: str, position: int, limit: int) -> List[Chunk]:
-        return [Chunk(**d) for d in self._db('list_chunks_after', document_id, position, limit)]
-
-    def list_chunks_before(self, document_id: str, position: int, limit: int) -> List[Chunk]:
-        return [Chunk(**d) for d in self._db('list_chunks_before', document_id, position, limit)]
-
     def list_collections_for_document(self, document_id: str, offset: int, limit: int) -> List[CollectionInfo]:
         return [CollectionInfo(**d) for d in self._db('list_collections_for_document', document_id, offset, limit)]
 
     def list_documents_in_collection(self, collection_id: str, offset: int, limit: int) -> List[DocumentInfo]:
         return [DocumentInfo(**d) for d in self._db('list_documents_in_collection', collection_id, offset, limit)]
 
     def list_jobs(self) -> List[Job]:
```

## Comparing `h2o_helium-0.4.0.dist-info/METADATA` & `h2o_helium-0.5.0.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: h2o-helium
-Version: 0.4.0
+Version: 0.5.0
 Summary: Client library for H2O Helium
 Author-email: Prithvi Prabhu <prithvi.prabhu@gmail.com>
 Project-URL: Source, https://github.com/h2oai/helium
 Project-URL: Issues, https://github.com/h2oai/helium/issues
 Project-URL: Documentation, https://github.com/h2oai/helium/wiki
 Keywords: information-retrieval,LLM,large-language-models,question-answering,search,semantic-search,analytical-search,lexical-search,document-search,natural-language-querying
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
+Requires-Dist: pydantic[dotenv] (~=1.10)
 Requires-Dist: requests
 Requires-Dist: websockets
-Requires-Dist: pydantic
 
 # H2O Helium Python Client
 
 ## Install
 
 ```bash
 pip install h2o-helium
```

